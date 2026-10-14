# Lab 5: Static Code Analysis — Reflection

### 1. What is static code analysis, and why is it useful?

Static code analysis examines source code without executing it to identify potential bugs, security vulnerabilities, and coding-style problems. It helps improve code quality, security, and maintainability.

### 2. What is the purpose of Pylint, Bandit, and Flake8?

Pylint checks code quality and programming practices. Bandit identifies common security vulnerabilities. Flake8 checks Python code style, formatting, and whitespace. Using all three provides different types of checks.

### 3. What issues did you identify and fix in your program?

I identified SQL injection risk, unsafe shell-command execution, overly broad exception handling, inconsistent function naming, missing docstrings, and formatting problems. I used parameterized SQL queries, removed shell-command execution, improved exception handling, followed snake_case naming, added docstrings, and corrected formatting.

### 4. What did you learn from this lab?

I learned that a program can run correctly and still contain security and code-quality problems. Static analysis tools help identify these problems early. After correcting my code, Pylint gave a score of 10/10, Bandit reported no security issues, and Flake8 reported no style violations.