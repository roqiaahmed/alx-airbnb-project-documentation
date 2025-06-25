# alx-airbnb-project-documentation

## User Authentication

- requirement tools: jwt, database storage.
- API endpoints:
  | endpoints | input | output |
  | ------------- | ------------- |--------------------- |
  | post /login | email&password| token & refreshToken |
  | post /signin | userInfo | token & refreshToken |

## Property Management

- requirement tools: database storage
- API endpoints:
  | endpoints | input | output |
  | ------------------------|-------------------|------------------------ |
  | post /property | property details | prooperty id |
  | update /property/:id |updated property | updated property value |
  | get /property/:id | - | property. |
  | delete /property/:id | - | deleted massage |

## Booking System

requirement tools: database storage, date validation library
API endpoints:
| endpoints | input | output |
|----------------------------|--------------------------------|----------------------------|
| post /booking | property_id, dates, guest_info | booking_id, confirmation |
| delete /booking/:id | cancellation_policy | cancellation_message |
| get /booking/:id/status | - | booking_status |
| get /bookings/property/:id | property_id | list_of_bookings |
