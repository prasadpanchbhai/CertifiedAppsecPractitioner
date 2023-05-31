# Understanding of OWASP Top 10 Vulnerabilities

<figure><img src=".gitbook/assets/image (14) (1).png" alt="" width="314"><figcaption></figcaption></figure>

### **What is OWASP?**

Open Web Application Security Project (OWASP) is an open community dedicated to raising awareness about security. OWASP created the top 10 lists for various categories in security.



### **What is the OWASP Top 10?**

Every few years, OWASP revises and publishes its list of the top 10 web **application vulnerabilities**. The list includes not only the OWASP Top 10 threats but also the potential impact of each vulnerability and how to avoid them. The comprehensive list is compiled from a variety of expert sources such as security consultants, security vendors, and security teams from companies and organizations of all sizes. It is recognized as an essential guide to web application security best practices.

OWASP has recently shared the 2021 OWASP Top 10 where there are three new categories, four categories with naming and scoping changes, and some consolidation within the Top 10.



### The Latest List of OWASP Top 10 Vulnerabilities and Web Application Security Risks

A newest OWASP Top 10 list came out on September 24, 2021 at the OWASP 20th Anniversary. If you’re familiar with the 2020 list, you’ll notice a large shuffle in the 2021 OWASP Top 10, as SQL injection has been replaced at the top spot by Broken Access Control.

1. Broken Access Control
2. Cryptographic Failures
3. **Injection**
4. Insecure Design
5. Security Misconfiguration
6. Vulnerable and Outdated Components
7. Identification and Authentication Failures
8. Software and Data Integrity Failures
9. Security Logging and Monitoring Failures
10. Server-Side Request Forgery



### OWASP Top 10 Vulnerabilities

**BROKEN ACCESS CONTROLS**

* Broken Access Control happens when access permissions are misconfigured thereby allowing attackers to access, modify or delete data, files and accounts that they should not have access to in the first place.
* Failures typically lead to unauthorized information disclosure or modification, destruction of data, or performing a business function outside the user’s limits.



**CRYPTOGRAPHIC FAILURES**

* Cryptographic failures occur when sensitive data is insufficiently protected and therefore leaked or exposed to unauthorized audiences. Such failures are most common if data is transmitted or stored in clear text or using known-to-be-weak cryptographic algorithms such as MD5 or SHA-1.



INJECTION

* An attacker can execute unintended commands or gain access to sensitive data by injecting malicious data as part of a command or query. This usually happens when a website fails to filter, validate or sanitize users’ inputs or implement parameterization.
* Injection vulnerabilities can occur when a query or command is used to insert untrusted data into the interpreter via [**SQL**](https://snyk.io/learn/sql-injection/), OS, NoSQL, or LDAP injection.



INSECURE DESIGN

* This newest OWASP Top 10 revision talks about risks related to design and architectural flaws, with recommendations for implementing threat modelling, secure design patterns, and reference architectures – from the very beginning of the design process.



SECURITY MISCONFIGURATION

* This category covers a brand range of potential vulnerabilities including insecure default configurations, open ports, incomplete configurations, and misconfigured HTTP headers, using insecure default usernames and passwords, etc.



VULNERABLE AND OUTDATED COMPONENTS

*   This refers to known issues where vulnerabilities exist because developers either do not know the versions of components used including those of nested dependencies, or are not aware that the software used is already unsupported or out of date.

    e.g. **Log4j2 Vulnerability**



IDENTIFICATION AND AUTHENTICATION FAILURES

* Previously known as “Broken Authentication”, this category covers weaknesses in authentication and session management in web applications. The resulting vulnerabilities allow attackers to gain unauthorized access to accounts and/or data.



SOFTWARE AND DATA INTEGRITY FAILURES

* For software, data integrity failures are becoming increasingly relevant as sensitive information is increasingly stored in databases, where it is at risk of tampering security.
* The section analyzes failures related to software updates (insufficient integrity verification), secure CI/CD pipelines, and the need for sufficient data integrity.
* Insecure Deserialization is now a part of Software and data integrity failure category.
* This is the second new category in the Top 10 in 2021, and is concerned with the failure to verify the integrity of software updates and patches prior to implementation on live applications and servers.



SECURITY LOGGING AND MONITORING FAILURES&#x20;

* Previously categorized as “Insufficient Logging and Monitoring”, Security Logging and Monitoring Failures moved one place up from #10 this year. Logging and monitoring are essential components in ensuring that any suspicious activity can be detected close to real-time, or diagnosed after the fact.



SERVER-SIDE REQUEST FORGERY (SSRF)

* Server-side request forgery (also termed as SSRF) is a web security flaw that allows an attacker to force a server-side application to send HTTP requests to any domain the attacker chooses
* When a web application fetches a remote resource without validating the user-supplied URL, an SSRF fault occurs. Even if the program is secured by a firewall, VPN, or another sort of network access control list, an attacker can force it to send a forged request to an unexpected location.
* This is the third and final new entry into the Top 10 in 2021. Server-Side Request Forgery (SSRF) occurs when a web application proceeds to fetch data without first validating user-supplied URL.

