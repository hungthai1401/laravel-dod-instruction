# Structure Rules

## General Standards:
- The application must follow a clean architecture with the following layers:
   - **Domain**: Contains core business logic, entities, value objects, and interfaces.
   - **Application**: Contains controllers, requests, and DTOs.
   - **Infrastructure**: Contains implementations of interfaces (e.g., repositories, external APIs).
   - **Support**: Contains utilities, and other supporting code.

## Folder Structure:
- **Domain Layer**:
   - Path: `src/Domain`
   - Subdirectories:
     - `Entities`: Core business entities.
     - `Actions`: Business logic encapsulated in action classes.
     - `DTOs`: Data Transfer Objects for passing data between layers.
     - `Repositories`: Interfaces for data access.

- **Application Layer**:
   - Path: `src/Application`
   - Subdirectories:
     - `Controllers`: Invokable controllers that delegate tasks to actions.
     - `Requests`: Form Request classes for validating incoming data.

- **Infrastructure Layer**:
   - Path: `src/Infrastructure`
   - Subdirectories:
     - `Repositories`: Implementations of repository interfaces defined in the Domain layer.
     - `Models`: Eloquent models for database interactions.

- **Support Layer**:
   - Path: `src/Support`
   - Subdirectories:
     - `Utilities`: Utility classes for common tasks.
     - `Formatters`: Classes for formatting data for output.

