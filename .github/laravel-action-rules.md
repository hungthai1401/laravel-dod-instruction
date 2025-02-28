# Action Rules

## General Standards:
- Actions must be placed in the `src/Domain` plus feature name directory and plus Actions directory.
- Each action should be encapsulated in a single class.
- Actions should handle specific business logic and return structured data.
- Use dependency injection to resolve dependencies such as repositories or external APIs.

## Method `execute`:
- All actions must implement a public method named `execute`.
- The `execute` method should accept parameters (e.g., DTOs) as input and return the result of the action.
- Avoid embedding request-specific logic in actions; instead, use DTOs to pass data.

## Additional Requirements:
- Include additional rules from [PHP Rules](./php-rules.md) for general PHP coding standards, performance optimization, and security best practices.
