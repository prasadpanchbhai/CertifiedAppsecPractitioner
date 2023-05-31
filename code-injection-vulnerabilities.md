# Code Injection Vulnerabilities

<figure><img src=".gitbook/assets/image (3).png" alt="" width="314"><figcaption></figcaption></figure>

**Code injection** is a type of attack in which an attacker injects malicious code into an application or system to execute arbitrary commands and gain unauthorized access to sensitive data. This type of attack is particularly dangerous because it can lead to data theft, system disruption, and even total system compromise.

Some of the code injection vulnerabilities are:

1. **SQL Injection** - This type of attack occurs when a malicious user enters SQL code into an input field, which can potentially allow them to gain access to sensitive information.
2. **Command Injection** - This type of attack occurs when a malicious user enters a command into an input field, which can be executed on the server.
3. **LDAP Injection** - This type of attack occurs when a malicious user enters Lightweight Directory Access Protocol (LDAP) code into an input field, which can be used to gain access to sensitive information.
4. **XPath Injection** - This type of attack occurs when a malicious user enters an XML Path Language (XPath) expression into an input field, which can be used to gain access to sensitive information.
5. **XML Injection** - This type of attack occurs when a malicious user enters code into an XML document, which can be used to gain access to sensitive information.
6. **Cross-Site Scripting (XSS)** - This type of attack occurs when a malicious user enters a malicious script into an input field on a web page, which can be used to gain access to sensitive information.
7. **SSI Injection** - This type of attack occurs when a malicious user enters a Server Side Include (SSI) command into an input field, which can be used to gain access to sensitive information.
8. **Format String Attack** - This type of attack occurs when a malicious user enters a formatted string into an input field, which can be used to gain access to sensitive information.
9. **Expression Language Injection** - This type of attack occurs when a malicious user enters an expression language code into an input field, which can be used to gain access to sensitive information.
10. **CRLF Injection** - This type of attack occurs when a malicious user enters a carriage return and line feed (CRLF) code into an input field, which can be used to gain access to sensitive information.



### **Command Injection vs. Code Injection Technique**

While they are often confused, a Code Injection differs from a **Command Injection vulnerability.** **Code Injection** is a collection of techniques that allow a malicious user to add his arbitrary code to be executed by the application. Code Injection is limited to target systems and applications since the code’s effectiveness is confined to a particular programming language.

On the other hand, **Command Injection** involves taking advantage of application vulnerabilities to extend its functionality so it can execute arbitrary commands. With command injection, attackers supply unsafe input to the system shell to execute OS commands on the vulnerable application.&#x20;

### **Mitigate Code Injection Attacks**

1. **Validate User Input** - Ensure that all user input is properly validated to prevent malicious code from being injected.
2. **Enforce Strict Access Controls** - Establish strict access controls to limit who can access sensitive data and systems.
3. **Encrypt Sensitive Data** - Encrypt sensitive data to protect it from unauthorized access.
4. **Update Software** - Ensure that all software is kept up to date to reduce the risk of an attack.
5. **Restrict Database Access** - Restrict access to databases to only those users who need it.
