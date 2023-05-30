# SQL Injection

<figure><img src=".gitbook/assets/image (13).png" alt="" width="314"><figcaption></figcaption></figure>

SQL injection is a type of attack that takes advantage of the structure of SQL to inject malicious code into a web application. It is one of the most common security vulnerabilities in web applications and can cause data loss, system compromise, and other malicious activities.

SQL injection attacks can be divided into three categories:

1. **Classic SQL injection**: Classic SQL injection involves manipulating the syntax of an SQL query to gain access to sensitive data. This typically involves entering malicious code into an input field or URL.
2. **Blind SQL injection**: Blind SQL injection is a type of attack that is used when the attacker does not have direct access to the database. In this case, the attacker will use techniques such as Boolean-based and time-based SQL injection to gain access to the database.
3. **Second-order SQL injection**: Second-order SQL injection is a type of attack that occurs when an attacker is able to inject malicious code into a web application and it is then executed when the application is used by another user.

In addition to these three types of attacks, there are also other methods of SQL injection. These include exploiting stored procedures, exploiting user-defined functions, exploiting remote command execution, and exploiting web application firewalls.

Examples of SQL injection include:

* **Inserting malicious code into an input field**: This involves entering malicious code into an input field in order to gain access to sensitive data. For example, an attacker may enter the following code into a login form:

```
SELECT * FROM users WHERE username='$username' AND password='$password' OR '1'='1'
```

* **Exploiting stored procedures**: This involves exploiting the stored procedures of a web application in order to gain access to sensitive data. For example, an attacker may use the following code to execute a stored procedure:

```
EXEC sp_executesql 'SELECT * FROM users WHERE username='$username' AND password='$password' OR '1'='1'
```

* **Exploiting user-defined functions**: This involves exploiting user-defined functions in order to gain access to sensitive data. For example, an attacker may use the following code to execute a user-defined function:

```
SELECT dbo.fn_getuserdata('$username','$password')
```

* **Exploiting remote command execution**: This involves exploiting the remote command execution feature of a web application in order to gain access to sensitive data. For example, an attacker may use the following code to execute a remote command:

```
EXEC xp_cmdshell 'SELECT * FROM users WHERE username='$username' AND password='$password' OR '1'='1'
```

* **Exploiting web application firewalls**: This involves exploiting the web application firewalls of a web application in order to gain access to sensitive data. For example, an attacker may use the following code to bypass a web application firewall:

```
SELECT * FROM users WHERE username LIKE '%$username%' AND password LIKE '%$password%'
```

SQL injection is a serious security risk and can have serious consequences for both the attacker and the victim. It is important to be aware of the different types of SQL injection and to take steps to prevent them. Some of them are as follows:

1. **Use parameterized queries** - Parameterized queries are a type of query that uses placeholders to represent values and prevent malicious code from being injected into the query.
2. Use prepared statements - Prepared statements are a type of query that is pre-compiled and can be used multiple times with different parameters.
3. Use input validation - Input validation is a technique that checks user input for malicious code and prevents it from being executed.
4. Implement whitelisting - Whitelisting is a technique that allows only certain data types and values to be accepted by the application.
5. Use stored procedures - Stored procedures are a type of query that is stored in the database and can be used to execute multiple queries in a single statement.
6. Encrypt sensitive data - Encryption is a technique that is used to protect sensitive data from being accessed by unauthorized users.
7. Use least privilege access - Least privilege access is a security principle that grants users the minimum access required to perform tasks.
8. Monitor system logs - System logs are a type of log that can be used to monitor system activity and detect suspicious activities.
9. Use web application firewalls - Web application firewalls are a type of firewall that is used to protect web applications from malicious traffic.
