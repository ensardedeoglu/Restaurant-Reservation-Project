
## Restaurant Reservation

# A Restaurant Reservation System intended for internal use by restaurant employees. 

[Restaurant Reservation System](https://front-end-lime-one.vercel.app/)

## 💻 Technology Used

> HTML, CSS, JavaScript, React, Express, Node.js, PostgreSQL, Knex.js, React Bootstrap, and Bootstrap 4.

## 📸 Screenshots

![Dashboard Tables and Reservations](https://i.imgur.com/Aq8OQVp.png)
![Create a New Reservation](https://i.imgur.com/KgXjmns.png)

## API Documentation

| Route                                | Method | Success Status Code | Description                                                                               |
| ------------------------------------ | ------ | ------------------- | ----------------------------------------------------------------------------------------- |
| /reservations                        | GET    | 200                 | Returns all reservations for specified date, ordered by reservation time.                 |
| /reservations                        | POST   | 201                 | Create a new reservation.                                                                 |
| reservations/:reservation_id         | GET    | 200                 | Return a specified reservation by ID.                                                     |
| reservations/:reservation_id         | PUT    | 200                 | Update an already existing reservation by ID.                                             |
| /reservations?date=YYYY-MM-DD        | GET    | 200                 | Returns all reservations for the specified date.                                          |
| /reservations/:reservation_id/status | PUT    | 200                 | Update status' of specified reservation between: booked, seated, cancelled, and finished. |
| /tables                              | GET    | 200                 | Returns all existing tables.                                                              |
| /tables                              | POST   | 201                 | Create a new table.                                                                       |
| /tables/:table_id                    | POST   | 201                 | Return a specified table by ID.                                                           |
| /tables/:table_id/seat               | PUT    | 200                 | Update status' of specified table between: occupied and free.                             |
| /tables/:table_id/seat               | DELETE | 200                 | Deletes occupied status and sets status to be free for specified table.                   |
