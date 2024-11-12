# Event Booking REST API

A Go-powered "EVENT BOOKING" REST API.

## API Endpoints

### Events

- **GET /events**  
  Get a list of available events.

- **GET /events/{id}**  
  Get details of a specific event by ID.

- **POST /events**  
  Create a new bookable event (authentication required).

- **PUT /events/{id}**  
  Update an existing event (authentication required, only by the creator).

- **DELETE /events/{id}**  
  Delete an event (authentication required, only by the creator).

### User Authentication

- **POST /signup**  
  Create a new user.

- **POST /login**  
  Authenticate user and obtain a JWT token.

### Event Registration

- **POST /events/{id}/register**  
  Register a user for an event (authentication required).

- **DELETE /events/{id}/register**  
  Cancel registration for an event (authentication required).

## Authentication

All endpoints marked with **(authentication required)** require a valid JWT token in the `Authorization` header.

## Setup and Run

1. Clone the repository.
2. Install dependencies.
3. Run the server.

```bash
go run main.go
