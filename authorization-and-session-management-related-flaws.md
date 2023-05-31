# Authorization and Session Management related flaws

<figure><img src=".gitbook/assets/image (14).png" alt="" width="314"><figcaption></figcaption></figure>

### **History of Authorization and Session Management Related Flaws**

The concept of authentication and authorization has been around since the early days of computing. Authentication is the process of verifying that a user is who they claim to be, while authorization is the process of determining what a user is allowed to do within a system. Authorization related flaws began to appear in the late 1990s and early 2000s, when the internet began to be used for more than just email and web browsing.

Early authorization related flaws included Insecure Direct Object Reference (IDOR), which allowed attackers to access resources to which they should not have access, and Insufficient Authorization, which allowed attackers to gain unauthorized access to restricted areas of an application. These types of vulnerabilities were often exploited by attackers to gain unauthorized access to a system or application, or to execute unauthorized actions on behalf of a user.

As the use of the internet and applications grew, so did the sophistication of the attacks, and Session Fixation and Session Hijacking became more common. Session Fixation occurs when an application does not properly manage session identifiers, allowing an attacker to fixate a session identifier and reuse it to gain unauthorized access. Session Hijacking occurs when an attacker is able to gain access to a user's session by stealing or predicting the session identifier.

In recent years, Cross-Site Request Forgery (CSRF) has become a more common type of authorization related flaw, as it allows an attacker to execute unauthorized actions on behalf of a user. As the use of the internet and applications continues to grow, these types of flaws will likely continue to evolve and become more sophisticated.

### **Authorization Related Flaws**

Authorization related flaws are security vulnerabilities that can occur when an application does not properly validate parameters used to access resources, authenticate users, or enforce authorization rules. These flaws can be exploited by attackers to gain unauthorized access to a system or application, or to execute unauthorized actions on behalf of a user.

Common Authorization related flaws include:

* **Insecure Direct Object Reference (IDOR):** IDOR flaws occur when the application does not properly validate parameters used to access resources, allowing an attacker to access objects or data to which they should not have access.
* **Broken Authentication and Session Management:** Broken Authentication and Session Management occurs when authentication and session management mechanisms are improperly implemented or configured, allowing an attacker to gain access to the application.
* **Insufficient Authorization:** Insufficient Authorization is when an application does not properly enforce authorization rules or limits on user access, allowing an attacker to gain unauthorized access.
* **Cross-Site Request Forgery (CSRF):** CSRF flaws occur when an application does not properly validate user requests, allowing an attacker to execute unauthorized actions on behalf of the user.

#### **Examples**

* A web application that does not properly validate user input and allows an attacker to bypass authentication and access sensitive data.
* A web application that does not properly implement authentication mechanisms, allowing an attacker to gain access to the application.
* An application with insufficient authorization rules, allowing an attacker to access restricted areas of the application.
* A web application that does not validate user requests, allowing an attacker to execute unauthorized actions on behalf of the user.



### **Session Management Flaws in Detail**

Session management flaws are security vulnerabilities that can occur when an application does not properly manage user sessions. These flaws can be exploited by attackers to access a system or application, or to execute unauthorized actions on behalf of a user.

Common session management flaws include:

* **Session Fixation:** Session Fixation occurs when an application does not properly manage session identifiers, allowing an attacker to fixate a session identifier and reuse it to gain unauthorized access.
* **Session Hijacking:** Session Hijacking occurs when an attacker is able to gain access to a user's session by stealing or predicting the session identifier.
* **Broken Authentication and Session Management:** Broken Authentication and Session Management occurs when authentication and session management mechanisms are improperly implemented or configured, allowing an attacker to gain access to the application.

#### **Examples**

* A web application that does not properly manage session identifiers, allowing an attacker to fixate a session identifier and reuse it to gain unauthorized access.
* A web application that does not properly implement authentication mechanisms, allowing an attacker to hijack a user's session.
* A web application that does not adequately protect session identifiers, allowing an attacker to easily steal or predict the session identifier.
