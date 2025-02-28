# DTO Rules

## General Standards:
- Actions must be placed in the `src/Domain` plus feature name directory and plus DTOs directory.
- DTOs should encapsulate and validate data from requests.
- Use immutable properties (e.g., `readonly` in PHP 8.1) to ensure data integrity.

## Structure:
- DTOs should have a constructor that accepts all required properties.
- Avoid adding business logic to DTOs; they should only represent data.

## Additional Requirements:
- Include additional rules from [PHP Rules](./php-rules.md) for general PHP coding standards, performance optimization, and security best practices.
