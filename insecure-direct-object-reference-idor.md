# Insecure Direct Object Reference (IDOR)

<figure><img src=".gitbook/assets/image (5).png" alt="" width="314"><figcaption></figcaption></figure>

Insecure direct object reference (IDOR) is an attack vector used by malicious actors to gain access to data or resources that should otherwise remain hidden. IDOR occurs when a web application does not adequately check user input before allowing access to a protected resource. This type of attack can occur when an application uses a user-supplied identifier to access a resource without proper authorization checks.

IDOR attacks can be broken down into three main types:

1. **Weak Identifier Use**: This occurs when an application uses weak identifiers, such as sequential numbers, to access a resource. This type of attack is particularly effective when the numerical sequence is predictable, allowing the attacker to guess the identifier and gain access to a protected resource.
2. **Incorrect Permission Assignment**: This type of IDOR attack occurs when an application assigns incorrect permissions to a user, allowing them to access resources that they are not authorized to access. This type of attack is especially dangerous as attackers can gain access to high-value resources, such as user databases.
3. **Inadequate Access Control**: This type of attack occurs when an application does not check the user’s identity before allowing access to a resource. This type of attack can be especially dangerous if the application is not properly secured, as attackers can easily gain access to the protected resource.

For example, if an application uses a numerical identifier to access a user’s account, an attacker can guess the user’s numerical identifier and gain access to their account without proper authorization checks.



### **Four common types of IDOR**

These days, identifiers are more commonly found in headers or APIs than right in a user’s address bar. However, the dynamic nature of most websites means that identifiers and parameters are still heavily used in some form or another. Identifiers might include:

* Database keys
* Query parameters
* User or session IDs
* Filenames

### **Mitigating IDOR Attacks**

IDOR attacks can be mitigated through the following steps:

1. **Ensure Strong Identifier Use**: Ensure that identifiers used to access resources are strong and difficult to guess. Examples of strong identifiers include random numbers or strings of characters.
2. **Properly Assign Permissions**: Ensure that user permissions are properly assigned and checked before granting access to a resource.
3. **Implement Access Controls**: Implement access controls to ensure that users are only able to access resources that they are authorized to access.
4. **Enforce Security Policies**: Implement and enforce security policies to ensure that the application is properly secured and that all user input is properly checked.
