# Repository Rules

## General Standards:
- Repository interfaces should be defined in the Domain layer.
- Repository interfaces should be implemented in the Infrastructure layer.
- Repository interfaces should define methods for interacting with data without specifying implementation details.
- Avoid embedding framework-specific logic (e.g., Eloquent) in repository interfaces.

## Method Definitions:
- Define methods for common CRUD operations:
   - `create(array $data): mixed`
   - `find(int $id): ?object`
   - `update(int $id, array $data): bool`
   - `delete(int $id): bool`
- Additional methods can be defined based on specific business requirements.

## Naming Conventions:
- Repository interfaces should be named suffixed with `Contract`.
- Use the suffix `Repository` for all repository interfaces (e.g., `PostRepository`, `UserRepository`).
- Method names should be descriptive and reflect their purpose (e.g., `findBySlug`, `getAllActivePosts`).

## Additional Requirements:
- Ensure compatibility with Dependency Injection principles.