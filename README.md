This document gives details about the Illis - Heka project. 

# Table of content
<!-- vim-markdown-toc GFM -->

- [Illis](#illis)
    - [Industry description](#industry-description)
- [Heka](#heka)
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
- V1 -> send payment notification

### User update popup

- Some fields not possible to change

## Property flow

V1 -> lock properties ( it will not be able to add or bulk add, just possible to update)
V1 -> schema generation of the properties tree schema?

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
- V1-> if locked doesn’t allow to change some fields
- Delete property 

## Financial flow

No sub menu

### Financial Main Page
- bar chart of balance time interval can change to week, month, quarter, year
- Paginated income and outbound sorted from latest created to oldest
- Filtering start and end date 
- V1 -> Button to take the sum of filtered or all 

### Financial detail page

- details of the payment fields
- Update?

## Calendar

V1 -> dynamic calendar with month week day selection

- month overview calendar 
- Left and right arrows to switch between months
- Events are stacked in the day if there is multiple
- Add event
- When event box is clicked popup to details

### Add event 

V1 -> notify option
Related user’s options 

- title, body, start date and duration, recurring dropdown( daily, weekly, monthly, yearly) interval.

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








