# Parameter Manipulation attacks

<figure><img src=".gitbook/assets/image (14).png" alt="" width="314"><figcaption></figcaption></figure>



Parameter manipulation attacks are a type of attack that targets application parameters, such as query strings, cookies, and form values. These attacks can be used to modify the application’s normal behavior and can have devastating effects, ranging from data corruption to account hijacking.

The most common type of parameter manipulation attack is a SQL Injection attack. In this type of attack, the attacker attempts to inject malicious SQL statements into an application parameter. For example, an attacker might attempt to inject a statement like “DROP TABLE users” into a field that expects a user ID. If the application isn’t properly sanitizing input, the statement may be executed, resulting in the destruction of all user accounts in the database.

Another type of parameter manipulation attack is a Cross-Site Scripting (XSS) attack. In this type of attack, the attacker attempts to inject malicious JavaScript code into an application parameter. This code can be used to execute malicious code on the user’s machine, or to redirect the user to a malicious website. For example, an attacker could inject a statement like “\<script>window.location = '[http://malicious.site/](http://malicious.site/)'\</script>” into an application parameter. If the application isn’t properly sanitizing input, the statement may be executed, resulting in the user being redirected to a malicious website.

In real life, parameter manipulation attacks have had serious consequences. In 2020, a hacker was able to use a parameter manipulation attack to access the personal information of more than 100 million users of the credit scoring company Equifax. In 2017, the fast food chain Wendy’s was the victim of a parameter manipulation attack that resulted in the theft of more than 1,000 customer credit and debit card numbers.

### **The Top 10 Types of Parameter Manipulation Attacks**

1. **SQL Injection**: In this type of attack, the attacker attempts to inject malicious SQL statements into an application parameter. For example, an attacker might attempt to inject a statement like “DROP TABLE users” into a field that expects a user ID.
2. **Cross-Site Scripting (XSS)**: In this type of attack, the attacker attempts to inject malicious JavaScript code into an application parameter. This code can be used to execute malicious code on the user’s machine, or to redirect the user to a malicious website.
3. **LDAP Injection**: This type of attack is similar to SQL injection, but instead of targeting a SQL database, the attacker targets an LDAP directory.
4. **HTML Injection**: This type of attack involves injecting malicious HTML code into an application parameter. This code can be used to modify the content or design of the page.
5. **Buffer Overflow**: In this type of attack, the attacker attempts to send more data than the application can handle. If the application isn’t properly sanitizing input, the extra data can be used to overwrite existing data or execute malicious code.
6. **URL Redirection**: In this type of attack, the attacker attempts to inject malicious code into an application parameter that will redirect the user to a malicious website.
7. **Session Hijacking**: In this type of attack, the attacker attempts to steal a user’s session ID and use it to gain access to the application.
8. **Cookie Stealing**: In this type of attack, the attacker attempts to steal a user’s cookie and use it to gain access to the application.
9. **Form Hijacking**: In this type of attack, the attacker attempts to submit malicious data through a form, such as a login form.
10. **Directory Traversal**: In this type of attack, the attacker attempts to access sensitive files or directories on the server.

Parameter manipulation attacks are a serious threat, and it’s important for developers to take steps to prevent them. Developers should make sure they are properly sanitizing all user input, and that they are using secure coding practices to ensure that malicious code can’t be injected into application parameters.

### **Mitigating Parameter Manipulation Attacks**

1. Properly sanitize all user input to prevent malicious code from being injected into application parameters.
2. Use secure coding practices to ensure that malicious code can’t be injected into application parameters.
3. Implement access control measures to limit who can access sensitive files or directories on the server.
4. Use encryption to protect sensitive data.
5. Use firewalls and other security measures to protect your applications from external threats.
6. Implement application whitelisting to limit the type of code that can be executed on the server.
