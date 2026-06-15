# SQL Injection on DVWA (Low Security)

## Objective

The objective of this project is to demonstrate a SQL Injection vulnerability using Damn Vulnerable Web Application (DVWA) running in Low Security mode.

## Tools Used

- DVWA (Damn Vulnerable Web Application)
- XAMPP
- Apache
- MySQL
- Web Browser

## Vulnerability Overview

SQL Injection is a web application vulnerability that occurs when user input is directly inserted into SQL queries without proper validation or sanitization.

## Setup Procedure

1. Started Apache and MySQL services using XAMPP.
2. Opened DVWA in a web browser.
3. Created the database using Setup / Reset Database.
4. Logged into DVWA.
5. Set the Security Level to Low.

## Payload Used

```sql
1' OR '1'='1
```

## Steps Performed

1. Opened the SQL Injection module.
2. Entered the payload in the User ID field.
3. Clicked Submit.
4. Observed multiple user records being returned.

## Results

The SQL Injection attack was successful. Multiple user records were displayed instead of a single record.

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
- Sensitive Information Disclosure
- Database Manipulation

## Prevention Methods

- Prepared Statements
- Parameterized Queries
- Input Validation
- Input Sanitization

## Conclusion

This project successfully demonstrated a SQL Injection vulnerability in DVWA running with Low Security settings. The attack highlighted the importance of secure coding practices and proper input validation.
