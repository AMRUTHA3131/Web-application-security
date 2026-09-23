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
text
1' OR 1=1 

## Observation
The application processed the supplied input as part of the SQL
statement. This demonstrates the risk of SQL Injection when
user input is not properly separated from SQL commands.

## Mitigation
Use prepared statements or parameterized queries.

###### Example:
$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");
$stmt->execute([$id]);

Prepared statements separate SQL instructions from user-supplied
data and help prevent SQL Injection.

## Testing Environment
- Kali Linux
- DVWA
- Docker
- Localhost
- Controlled laboratory environment
