# G12 – TPI – Court Reservations

This README.md documents the Integrative Practical Project for Application Development with Objects, following the activity structure proposed by the course, including links and images corresponding to the required diagrams.

---

## Feature Overview

The system allows managing sports court reservations for a sports complex.

It is used to manage clients, courts, schedules, tournaments, and additional services (such as lighting or referees), ensuring court availability and preventing schedule overlaps. It also includes statistical reports about court utilization, and allows registering payments associated with reservations/tournaments.

The main **objective** is to digitize and optimize the reservation process, eliminating conflicts caused by overlapping time slots, providing clear information about court occupancy and billing.

---

## Use Cases

The functionalities we propose to implement are listed in the following table:

| Nº  | Use Case                                                   | Description                                                                                               |
| --- | ---------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| UC1 | **Register Client**                                       | Add a new client to the system, validating that the ID number is not duplicated.                         |
| UC2 | **Modify / Delete Client**                                | Update or delete existing client data.                                                                    |
| UC3 | **Register Court**                                        | Create a new court with its type, cost, and associated services.                                          |
| UC4 | **Modify Court Status**                                   | Update the status of a court.                                                                             |
| UC5 | **Register Reservation**                                  | Create a reservation linking client, court, date, and time. Availability is checked before confirmation. |
| UC6 | **Modify Reservation**                                    | Change schedule or cancel an existing reservation.                                                        |
| UC7 | **Check Availability**                                    | Display available courts for a date and time range.                                                       |
| UC8 | **Register Tournament**                                   | Create tournaments, assign courts, and link reservations.                                                 |
| UC9 | **Register Payment**                                      | Register a payment for a reservation or tournament (amount, date, method).                               |
| UC10| **Register Service**                                      | Register a service associated with a specific court.                                                      |
| UC11| **Generate Report of Reservations by Client**             | Generate a report listing all reservations made by a client.                                              |
| UC12| **Generate Report of Reservations by Court and Period**   | Generate a report of court reservations within a date range.                                              |
| UC13| **Generate Report of Most Used Courts**                   | Generate a report showing which courts are most frequently reserved.                                      |
| UC14| **Generate Monthly Usage Statistics Chart**               | Generate charts (bar or pie) showing monthly court utilization.                                           |

---

## Applied Design Pattern

We applied the **DAO pattern** to manage CRUD operations, separating business logic from persistence in the database, along with a **monolithic MVC architecture** for code organization.

![MVC Diagram](assets/imgs/mvc.jpg)

---

## Entity–Relationship Diagram

The ER diagram was created using **dbdiagram.io**. The proposed diagram is shown below:

![ER Diagram](assets/imgs/G12_TPI_DAO_DER.png)

---

## Class Diagram

The class diagram was built using **draw.io**. The proposed diagram is shown below:

![Class Diagram](assets/imgs/G12_DAO_Reservas_Canchas-diagrama-terminado.jpg)

---

## Team Members

| Student ID | Last Name, First Name      | Email                           |
| ---------- | ------------------------- | -------------------------------- |
| 93203      | Ceballos Pratto, Agustín | agusceballos000@gmail.com        |
| 95309      | Fernandez, Julian         | julianfernandez159155@gmail.com  |
| 94416      | Pecchio, Valentina        | valuupecchio@gmail.com           |
| 91541      | Villegas, Genaro          | gvillegaslearning@gmail.com      |
| 89390      | Wendler, Juan José        | juanjoowendler@gmail.com         |

---
