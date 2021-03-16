This document gives details about the Illis - Heka project. 

# Table of content
<!-- vim-markdown-toc GFM -->

- [Illis](#illis)
    - [Industry description](#industry-description)
- [Heka](#heka)
- [Design Choices](#design-choices)
- [Road map](#road-map)
- [MVP](#mvp)
    - [User Flow](#user-flow)
        - [Users Page](#users-page)
        - [Users Submenu](#users-submenus)
        - [Users Detail Popup](#users-detail-popup)
        - [Users Update Popup](#user-update-popup)
    - [Property Flow](#property-flow)
        - [Property Page](#properties-page)
        - [Property Submenu](#properties-submenus)
        - [Property Detail Popup](#property-details-popup)
        - [Property Update Popup](#property-update-popup)
    - [Financial Flow](#financial-flow)
        - [Main Page](#financial-main-page)
        - [Detail Page](#financial-detail-page)
    - [Calendar Page](#calendar)
        - [Add event](#add-event)
        - [Event Detail Popup](#event-details-popup)
    - [Settings Page](#settings)
- [V1](#v1)
    - [Ideas](#ideas)
        
        
# Illis

The parent company of the Heka property subscription management solution. 
Illis vision is to bring new technologies,
such as blockchain for rental aggrements and machine learning for automation of processes to the property market in Turkey.
Heka is the starting product for this journey. 

##### Industry description

In Turkey, Building or Building complexes has managers. 
Tenant or the owner obligated to pay subscription to the building for services. 
These services are garbage collection, maintanance of the garden, pool, elevator, parking. Some buildings or building 
complexes has security as well. 
Managers are responsible for collection of the subscription, subscription payer changes, new tenant registration,
workers organization, external vendor arrangements, maintanance planning. 

Currently, old overpriced desktop software or excel sheets are being used for this planning.

# Heka 

Heka is online platform to help the property managers to ease the management process. 

The main functionalities will be Dashboard, User Flow, Properties Flow, Financial flow, Calendar, Notification, Settings

# Design Choices

- Database: Postgres
- Backend: FastAPI Python, REST 
    - It is inhouse build
    - Current status: MVP functions are %70 ready
- Frontend: React Javascript, HTML, CSS(Framework flexible)

# Road Map

- Q1 2021 - MVP online
- Q2 2021 - Version 1 online
- Q3 2021 - Expantion starts
- Q4 2021 - Version 2 starts
- Q1 2022 - Possible buyer search

# MVP 

minimum viable product will consist of dashboard, user flow, properties flow, financial flow and calendar. 

## user flow

### Users page: 

- List users paginated
- Filter user based on column values( role type, ) 
- Search within users ( name surname details, nationalid)
- Add new user

### Users submenus:
- Role-types for distribution 
- No role-type filtering is needed 
- Search within users


### Users detail popup

- Update user
- Connect user to the property
- Add payment 
- Delete user

### User update popup

- Some fields not possible to change

## Property flow

### Properties page

- List all properties with pagination 
- Filter properties
- Search in properties ( which fields?)
- Add new properties

### Properties submenus
- Property type for distribution 
- No filtering is needed
- Search is possible

### Property details popup
- Update property
- Connect property to user
- Connect property to property

### Property update popup
- Delete property 

## Financial flow

No sub menu

### Financial Main Page
- bar chart of balance time interval can change to week, month, quarter, year
- Paginated income and outbound sorted from latest created to oldest
- Filtering start and end date 

### Financial detail page

- details of the payment fields
- Update? for now it is not available

## Calendar

- month overview calendar 
- Left and right arrows to switch between months
- Events are stacked in the day if there is multiple
- Add event
- When event box is clicked popup to details

### Add event 

Related user’s options 

- title, 
- body
- start date and duration
- recurring dropdown( daily, weekly, monthly, yearly) interval.

### event details popup

- Title, body start datetime, end datetime 
- Delete the event


## Settings

General settings for the distributions settings
form to show the current settings 
when the values are changed the save button

- official e-mail
- notification setting
    - send mail
    - sms
- super user

# V1

## ideas

**User flow**

- V1 -> send payment notification

**Property flow**

- V1 -> lock properties ( it will not be able to add or bulk add, just possible to update)
- V1 -> schema generation of the properties tree schema?
- Property update - V1-> if locked doesn’t allow to change some fields

**Financial flow**

- mainpage V1 -> Button to take the sum of filtered or all

**Calendar**

- V1 -> dynamic calendar with month week day selection
- add event: V1 -> notify option











