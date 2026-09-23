# SQL Injection

## Objective

To demonstrate SQL Injection in DVWA using a controlled local
laboratory environment.

## Attack Scenario

SQL Injection occurs when user-controlled input is directly
included in an SQL query without proper protection.

In the DVWA SQL Injection page, a test input was supplied through
the `id` parameter to demonstrate that the application's SQL query
could be manipulated.

### Test Input

```text
1' OR 1=1 #
