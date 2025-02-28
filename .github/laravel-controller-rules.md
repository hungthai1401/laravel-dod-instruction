# Controller Rules

## General Standards:
- Controllers must be placed in the `src/Application/Api` plus feature name directory.
- All controllers must be invokable, meaning they should only contain a single `__invoke` method.
- Validate incoming requests using Form Request classes or inline validation within the `__invoke` method.

## DTO Usage:
- All controllers must use Data Transfer Objects (DTOs) to encapsulate and process request data.
- All controllers must delegate business logic to Action Classes.
- The Action Class should be instantiated and its `execute` method called with the appropriate parameters (e.g., DTO).
- The DTO should be created from the incoming request and passed to service classes for business logic.

## Additional Requirements:
- Use dependency injection to resolve dependencies.
- Keep the `__invoke` method concise and focused on a single responsibility.

- Include additional rules from [PHP Rules](./php-rules.md) for general PHP coding standards, performance optimization, and security best practices.
