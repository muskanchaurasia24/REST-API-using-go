REST API using go

A Go-powered "EVENT BOOKING" Rest Api

GET/events                  ----> get a list of available events
GET/events/<id>             ----> get a list of available events
POST/events                 ----> Create a new bookable event **(auth required)**
PUT/events/<id>             ----> update an event **(auth required)(only by creator)**
DELETE/events/<id>          ----> delete an event **(auth required)(only by creator)**
POST/signup                 ----> create new user
POST/login                  ----> authenticate user **(auth token JWT)**
POST/evnts/<id>/register    ----> register user for event**(auth required)**
Delete/events/<id>/register ----> Cancel register **(auth required)**