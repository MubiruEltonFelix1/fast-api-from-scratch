# FastAPI From Scratch

> **Learn FastAPI by building your way from first principles to production-level intuition.**

A project-based learning roadmap for understanding **FastAPI**, modern Python APIs, and the ideas behind them—not just memorizing decorators and copying tutorials.

The repository is currently being prepared. **Projects are coming soon.**

---

## What this repository is supposed to do

This repository is designed to teach FastAPI progressively through increasingly capable projects.

Instead of starting with a large production template, you will begin with small, understandable experiments and gradually build toward complete backend systems. Each level is intended to answer three questions:

1. **What is happening?**
2. **Why does it work this way?**
3. **When would I use this in a real application?**

The goal is to build durable intuition around:

- HTTP and REST APIs
- Request and response lifecycles
- URL paths, query parameters, headers, and cookies
- JSON serialization and validation
- Python type hints and Pydantic models
- Dependency injection
- Authentication and authorization
- Databases and persistence
- Async programming
- Background work
- Testing and observability
- Deployment and production architecture

---

## What is FastAPI?

[FastAPI](https://fastapi.tiangolo.com/) is a modern Python web framework for building APIs and backend services.

It combines:

- **Python type hints** for clearer code and automatic validation
- **Starlette** for web handling and asynchronous capabilities
- **Pydantic** for data parsing and validation
- **Automatic OpenAPI documentation** for interactive API exploration
- **Excellent performance** for a Python web framework
- **A developer-friendly experience** for building typed, maintainable services

A minimal FastAPI application looks like this:

```python
from fastapi import FastAPI

app = FastAPI()


@app.get("/")
def read_root():
    return {"message": "Hello, FastAPI"}
```

FastAPI turns this small amount of code into an HTTP endpoint that can be called from a browser, frontend application, mobile app, command-line client, or another service.

---

## Who this repository is for

This repository is for learners who want to:

- Learn FastAPI from the ground up
- Understand backend concepts instead of only copying syntax
- Strengthen their Python skills through practical projects
- Build APIs for web and mobile applications
- Move from scripts to real services
- Learn how production APIs are structured
- Create a portfolio of progressively more advanced projects
- Develop the confidence to read unfamiliar backend code

### Helpful, but not required

You will benefit from knowing:

- Basic Python syntax
- Functions and modules
- Classes and objects
- Lists, dictionaries, and exceptions
- Basic command-line usage
- The general idea of a web browser and a server

No previous FastAPI experience is required.

---

## The learning philosophy

### Build intuition before abstraction

Every project should make the underlying mechanism easier to see. We will avoid hiding important concepts behind layers of boilerplate too early.

### Start small, then add pressure

A concept becomes clearer when the application has a reason to need it. The curriculum will introduce complexity only after the simpler version is understandable.

### Learn by changing things

Learners should be encouraged to modify routes, break validation, inspect responses, add logging, change data models, and observe what happens.

### Prefer working mental models

The objective is not to remember every FastAPI option. The objective is to know how to reason about a request moving through a system.

### Projects over isolated syntax

Each project should connect multiple concepts and produce something that behaves like a real service.

---

## Skill progression

The levels below are a playful progression system, not official FastAPI certifications.

| Level | Focus | Intended outcome |
|---|---|---|
| **Pre-Beginner** | First contact with web APIs | Understand what a server, route, and response are |
| **Beginner** | Core FastAPI building blocks | Build small typed APIs confidently |
| **Intermediate** | Real application structure | Add persistence, validation, and reusable components |
| **Pro** | Production-minded backend development | Build secure, tested, maintainable services |
| **Master** | Architecture and scale | Reason about complex systems and trade-offs |
| **Legend** | Deep systems thinking | Design resilient services with strong operational intuition |
| **Reid Wiseman Level** | Mission-ready execution | Operate calmly across complex, high-stakes backend scenarios |
| **Walter Bishop Mode** | Experimental mastery | Explore unusual ideas, advanced integrations, and unconventional solutions |

---

## Project roadmap

> All projects below are planned. **No projects have been implemented yet. Coming soon.**

### 0. Pre-Beginner — See the request

Projects at this level make the web visible.

Planned projects:

- **Hello API** — Create your first FastAPI app and route
- **Status Server** — Return service status and a health message
- **Personal Profile API** — Return structured information as JSON
- **Route Explorer** — Compare path parameters, query parameters, and fixed routes
- **Interactive Docs Tour** — Explore Swagger UI and ReDoc

Concepts introduced:

- What an API is
- HTTP methods
- URLs and routes
- JSON responses
- Running a local development server
- Automatic API documentation

---

### 1. Beginner — Learn the building blocks

Projects at this level introduce the core tools used in everyday FastAPI development.

Planned projects:

- **Todo API** — Create, read, update, and delete tasks in memory
- **Unit Converter API** — Validate inputs and return calculated results
- **Book Catalog API** — Use Pydantic models for request and response data
- **Polling API** — Accept votes and return simple summaries
- **Notes API** — Separate route logic from application setup

Concepts introduced:

- Request bodies
- Path and query parameters
- Pydantic models
- Response models
- Validation errors
- Status codes
- CRUD operations
- Basic project organization

---

### 2. Intermediate — Build an actual application

Projects at this level introduce persistence, relationships, reusable dependencies, and more deliberate architecture.

Planned projects:

- **Task Manager API** — Persist data in a relational database
- **Inventory API** — Model products, stock levels, and updates
- **Recipe API** — Add filtering, pagination, and search
- **Habit Tracker API** — Work with dates, users, and recurring records
- **Personal Finance API** — Add categories, summaries, and reporting endpoints

Concepts introduced:

- SQL databases
- SQLAlchemy or SQLModel
- Database sessions
- Migrations
- Relationships
- Pagination
- Filtering and sorting
- Dependency injection
- Service and repository layers
- Environment-based configuration

---

### 3. Pro — Build for real users

Projects at this level focus on security, testing, maintainability, and production-oriented behavior.

Planned projects:

- **Authentication Service** — Registration, password hashing, and token-based login
- **Team Workspace API** — Users, teams, roles, and permissions
- **File Upload Service** — Validate, store, and retrieve uploaded files
- **Notification API** — Queue and deliver application notifications
- **Event Booking API** — Handle availability, conflicts, and business rules
- **Production-Ready Blog API** — Combine users, posts, comments, search, and moderation

Concepts introduced:

- Authentication and authorization
- OAuth2 and JWT concepts
- Password security
- Role-based access control
- Automated testing
- Test databases and fixtures
- Error handling
- Structured logging
- CORS
- Rate limiting concepts
- Background tasks
- Containerized development

---

### 4. Master — Think in systems

Projects at this level explore architecture, boundaries, resilience, and collaboration between services.

Planned projects:

- **Modular Marketplace API** — Separate catalog, orders, payments, and users
- **Real-Time Collaboration Service** — WebSockets and connected clients
- **Document Processing Pipeline** — Upload, queue, process, and report status
- **Analytics Ingestion API** — Accept events and generate aggregates
- **Multi-Tenant SaaS Backend** — Isolate organizations and their data
- **API Gateway Playground** — Route requests across multiple services

Concepts introduced:

- Modular monoliths
- Service boundaries
- WebSockets
- Message queues
- Event-driven workflows
- Idempotency
- Transactions
- Caching
- Distributed tracing concepts
- Multi-tenancy
- API versioning
- Resilience and failure handling

---

### 5. Legend — Design for failure

Projects at this level are designed around real operational problems rather than happy-path demos.

Planned projects:

- **Resilient Order Platform** — Retries, idempotency, and partial failures
- **Distributed Job Runner** — Schedule, execute, retry, and inspect jobs
- **High-Volume Metrics API** — Ingest and query large event streams
- **Incident Management API** — Track alerts, responders, timelines, and recovery
- **Service Reliability Lab** — Add health checks, metrics, tracing, and controlled failure

Concepts introduced:

- Backpressure
- Retries and exponential backoff
- Circuit breakers
- Dead-letter queues
- Graceful degradation
- Health and readiness checks
- Metrics and observability
- Load testing
- Capacity planning
- Data consistency trade-offs
- Disaster recovery thinking

---

### 6. Reid Wiseman Level — Mission-ready execution

This level is about combining technical depth with calm, disciplined execution. Projects simulate complex environments where requirements change, systems fail, and the API must remain understandable.

Planned projects:

- **Mission Control API** — Coordinate tasks, telemetry, users, and system status
- **Remote Operations Platform** — Manage commands, permissions, acknowledgements, and audit trails
- **Resource Allocation System** — Handle competing priorities and constrained resources
- **Live Operations Dashboard Backend** — Combine real-time updates with historical records
- **Recovery Scenario Simulator** — Practice safe failure handling and service restoration

Focus areas:

- Clear operational contracts
- Auditability
- Safe changes
- Explicit state transitions
- Runbooks and incident response
- Data integrity under pressure
- Real-time system behavior
- Communication between services and operators

---

### 7. Walter Bishop Mode — Experimental mastery

This is the laboratory tier: advanced, strange, ambitious, and intentionally exploratory.

Planned projects:

- **Federated Knowledge API** — Search and combine multiple knowledge sources
- **Agent Workflow Backend** — Coordinate long-running, tool-using workflows
- **Time-Window Event Engine** — Process events based on temporal rules
- **Experimental Graph API** — Model relationships between people, objects, and events
- **Self-Observing Service** — Build an API that explains its own requests, failures, and performance
- **Impossible Requirements Lab** — Solve deliberately unusual backend constraints

Focus areas:

- Advanced async workflows
- Event sourcing concepts
- Graph-shaped data
- Pluggable architectures
- Dynamic workflows
- Experimental interfaces
- Safe handling of uncertainty
- Knowing when not to over-engineer

---

## What each future project should contain

Each project is intended to include more than source code. A complete project should eventually include:

- A clear problem statement
- A short architecture explanation
- A working FastAPI application
- Example requests and responses
- A documented API surface
- Setup instructions
- Tests
- Common mistakes and debugging notes
- Exercises for extending the project
- “Break it on purpose” experiments
- A reflection section explaining the intuition learned

---

## Suggested repository structure

The repository is currently a roadmap. As projects are added, the structure may grow toward something like this:

```text
fastapi-from-scratch/
├── README.md
├── pyproject.toml
├── lessons/
│   ├── 00-pre-beginner/
│   ├── 01-beginner/
│   ├── 02-intermediate/
│   ├── 03-pro/
│   ├── 04-master/
│   ├── 05-legend/
│   ├── 06-reid-wiseman-level/
│   └── 07-walter-bishop-mode/
├── projects/
│   ├── pre-beginner/
│   ├── beginner/
│   ├── intermediate/
│   ├── pro/
│   ├── master/
│   ├── legend/
│   ├── reid-wiseman-level/
│   └── walter-bishop-mode/
├── shared/
│   ├── testing/
│   ├── configuration/
│   └── utilities/
└── docs/
    ├── http-intuition.md
    ├── fastapi-concepts.md
    └── production-notes.md
```

This structure is proposed for the learning journey and may change as implementation begins.

---

## Technology direction

The primary focus is FastAPI and modern Python backend development. Future projects may use tools such as:

- Python
- FastAPI
- Pydantic
- Uvicorn
- SQLAlchemy or SQLModel
- PostgreSQL
- Alembic
- Pytest
- Docker
- Redis
- Celery or another task-processing approach

Specific tools will be introduced when a project needs them. The repository will avoid adding infrastructure merely for appearance.

---

## Current status

**Status: Planning / coming soon**

The repository currently contains the learning direction and project roadmap. The projects have not been implemented yet.

Planned next steps:

- [ ] Add the first pre-beginner lesson
- [ ] Add the Hello API project
- [ ] Document the local development setup
- [ ] Add beginner exercises
- [ ] Add tests alongside the first projects
- [ ] Expand the project notes after each implementation

---

## How to use this repository when projects arrive

For each level:

1. Read the concept introduction.
2. Build the smallest version of the project.
3. Run it locally and inspect the requests and responses.
4. Change the code intentionally.
5. Break validation and error handling on purpose.
6. Complete the exercises.
7. Read the solution only after attempting the challenge.
8. Write down what changed in your mental model.

The best outcome is not finishing every project quickly. It is becoming able to look at a backend system and explain what it is doing.

---

## Contributing

This repository is primarily a learning project, but suggestions, corrections, exercises, and project ideas are welcome.

When contributing:

1. Keep explanations beginner-friendly without removing technical accuracy.
2. Prefer small, focused examples.
3. Explain the reason behind a pattern, not only the pattern itself.
4. Include tests or reproducible examples where appropriate.
5. Avoid introducing abstractions before they solve a demonstrated problem.

---

## License

A license will be added when the repository’s sharing and contribution terms are finalized.

---

## Final objective

By the end of this journey, you should be able to:

- Build a FastAPI service from an empty directory
- Explain how an HTTP request moves through the application
- Design clear request and response contracts
- Validate data confidently
- Connect an API to a database
- Secure routes and manage permissions
- Test behavior instead of guessing
- Diagnose failures systematically
- Choose appropriate architecture for the problem
- Know when a simple solution is better than a clever one

> **Start with a route. End with intuition.**
