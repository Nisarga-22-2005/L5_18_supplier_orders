# Static Code Analysis Issues

| No. | Tool | Line | Issue | Severity | Suggested Fix |
|---:|---|---:|---|---|---|
| 1 | Bandit | 21 | Use of `os.system()` with string concatenation can cause shell command injection. | High | Avoid shell execution and use a safer alternative. |
| 2 | Bandit | 11 | SQL query uses string formatting, creating a possible SQL injection risk. | Medium | Use parameterized SQL queries. |
| 3 | Bandit | 27–28 | Broad exception handling silently ignores errors. | Low | Handle specific exceptions and report errors appropriately. |
| 4 | Pylint | 10, 15, 20, 31 | Function names do not follow the snake_case naming convention. | Low | Rename functions using snake_case. |
| 5 | Pylint | Multiple | Functions are missing docstrings. | Low | Add short descriptions to functions. |
| 6 | Pylint | 31 | The `conn` parameter redefines a name from the outer scope. | Low | Use clear and consistent variable scope. |
| 7 | Flake8 | 5, 11, 32 | Lines exceed the recommended 79-character limit. | Low | Split long lines across multiple lines. |
| 8 | Flake8 | 12 | Missing whitespace around the `+=` operator. | Low | Write `order_total += quantity`. |

## Summary

Static analysis identified security risks, exception-handling problems, naming issues, and formatting violations. Bandit detected a high-severity shell command risk and a medium-severity possible SQL injection. These findings will guide the code improvements.