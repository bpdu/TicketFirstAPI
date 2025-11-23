# TicketFirstAPI

TicketFirstAPI is a backend service for a ticket-driven issue tracking system. It provides a clean and focused HTTP API for managing support tickets, agents, clients, and ticket comments, without any built-in frontend.

The project is designed as a learning and reference implementation of a CRUD-style application using **Python**, **FastAPI**, and **PostgreSQL**.

---

## Goals

- Explore modern backend development practices in Python.
- Build a concise, well-structured REST-style API.
- Gain hands-on experience with FastAPI and relational databases (PostgreSQL).
- Create a foundation that can be later integrated with any frontend or external systems.

---

## Core Concepts

TicketFirstAPI models a simple helpdesk / issue-tracking domain built around the following core entities:

- **Ticket**  
  Represents a single issue or request. A ticket can be created, updated, assigned to an agent and a client, and enriched with comments.

- **Agent**  
  A support representative responsible for handling tickets.

- **Client**  
  A person or system that creates tickets and for whom issues are resolved.

- **Comment**  
  A textual note attached to a ticket, used to track communication and progress.

These entities are exposed through a set of CRUD operations over HTTP.

---

## Features (Planned / Implemented)

- Create, read, update, and delete tickets.
- Assign or change:
  - the agent responsible for a ticket,
  - the client associated with a ticket,
  - the comment(s) attached to a ticket.
- Basic validation of input data.
- Clear separation between domain models and transport (API) models.
- Auto-generated interactive API documentation via FastAPI (OpenAPI/Swagger UI).

More advanced features (such as authentication, authorization, ticket statuses, priorities, tags, or SLA rules) can be added incrementally as the project evolves.

---

## Technology Stack

- **Language:** Python
- **Framework:** FastAPI
- **Database:** PostgreSQL
- **API Style:** REST-like JSON over HTTP

Additional tooling (such as Docker configuration, migrations, and testing frameworks) will be introduced as the project grows.

---

## Intended Use

TicketFirstAPI can be used as:

- A learning project for understanding backend architecture with FastAPI and PostgreSQL.
- A starting point for building a more complex internal support system.
- A backend service to be consumed by:
  - web frontends,
  - mobile applications,
  - automation scripts,
  - or other services.

---

## Project Status

This project is currently under active development and should be considered a work in progress.  
Breaking changes may occur while the API and data model are being refined.

---

## License

This project is licensed under the **MIT License**.  
You are free to use, modify, and distribute the code, both for personal and commercial purposes, without warranty of any kind.

