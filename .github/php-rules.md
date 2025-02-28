# PHP Rules

## General Coding Standards:
- Follow PSR-12 coding standards for consistent code formatting.
- Avoid hardcoding values; use configuration files or constants instead.
- Write clean and reusable code with proper error handling and logging.
- Use meaningful variable and function names that reflect their purpose.
- Ensure all code passes PHPStan static analysis at level 8 (the strictest level). Avoid writing code that triggers PHPStan errors or warnings.

## Performance Optimization:
- Optimize performance by avoiding unnecessary operations or loops.
- Use caching mechanisms where applicable to improve response times.
- All code you write MUST be fully optimized. ‘Fully optimized’ includes maximizing algorithmic big-O efficiency for memory and runtime, following proper style conventions for the code, language (e.g. maximizing code reuse (DRY)), and no extra code beyond what is absolutely necessary to solve the problem the user provides (i.e. no technical debt). If the code is not fully optimized, you will be fined $100.

## Security Best Practices:
- Always validate and sanitize user inputs to prevent SQL injection and XSS attacks.
- Use prepared statements or ORM tools to interact with the database securely.
- Implement proper error handling and avoid exposing sensitive information in error messages.