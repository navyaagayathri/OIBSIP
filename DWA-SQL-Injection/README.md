# SQL Injection on DVWA (Low Security)

## Objective

Demonstrate an SQL Injection vulnerability on a web application using DVWA (Damn Vulnerable Web Application) with the security level set to Low.

## Tools Used

- DVWA (Damn Vulnerable Web Application)
- XAMPP
- Apache
- MySQL
- Web Browser

## Setup

1. Installed and configured DVWA on a local server using XAMPP.
2. Started Apache and MySQL services.
3. Created the DVWA database using the Setup / Reset Database page.
4. Logged into DVWA using the default credentials.
5. Set the security level to Low using the DVWA Security page.

## Steps Performed

1. Opened the SQL Injection module in DVWA.
2. Entered a normal User ID (`1`) to observe the default behavior.
3. Entered the following SQL Injection payload:

```sql
1' OR '1'='1
```

4. Submitted the request.
5. Observed that the application returned multiple user records instead of a single record.

## Why This Works

At Low Security, DVWA directly inserts user input into SQL queries without proper validation or sanitization. The payload:

```sql
1' OR '1'='1
```

creates a condition that is always true, causing the database to return all matching records.

## Result

The SQL Injection attack was successful. Multiple user records were displayed, demonstrating that the application is vulnerable to SQL Injection attacks when user input is not properly handled.

## Screenshots

### Database Setup
- screenshots/01_database_setup.png

### Security Level Set to Low
- screenshots/02_security_level_low.png

### SQL Injection Payload
- screenshots/03_sql_injection_payload.png

### SQL Injection Result
- screenshots/04_sql_injection_result.png

## Impact of SQL Injection

- Authentication Bypass
- Unauthorized Data Access
- Information Disclosure
- Database Manipulation
- Potential System Compromise

## Prevention Methods

- Use Prepared Statements
- Use Parameterized Queries
- Validate User Input
- Sanitize User Input
- Follow Secure Coding Practices
- Apply Least Privilege Access Control

## Conclusion

This project successfully demonstrated a SQL Injection vulnerability in DVWA running with Low Security settings. The exercise highlights the importance of secure coding practices, input validation, and parameterized queries in protecting web applications against SQL Injection attacks.
