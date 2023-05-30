# Cross-Site Request Forgery

<figure><img src=".gitbook/assets/image (4).png" alt="" width="314"><figcaption></figcaption></figure>



Cross-Site Request Forgery (CSRF) is a type of attack which is carried out when an attacker tricks a user into sending a malicious request to a target website. This kind of attack is possible when a user is logged into a website and the attacker manipulates them into sending a request to the target website.

The malicious request can be a GET or POST request, and the attacker can use it to access and modify sensitive user data, or to execute unwanted commands on a vulnerable website. It is important to note that CSRF attacks are often hidden within legitimate requests, which makes them difficult to detect.

### **Examples of Cross-Site Request Forgery**

One example of a CSRF attack is a malicious actor manipulating a user into sending a POST request to a vulnerable website. The POST request could contain sensitive data, such as credit card information, which the attacker can then use to access the user's account or make purchases without their knowledge.

Another example of a CSRF attack is an attacker manipulating a user into sending a GET request to a vulnerable website. The GET request could contain a malicious command, such as “delete all users”, which the attacker can then use to delete all users from the website without the user’s knowledge.



## **What is the impact of a CSRF attack?**

The impact of a CSRF attack depends on the targeted user and their privileges within an application.

For the average user, a successful CSRF attack will typically introduce state-changing requests such as their password or email address being changed, their funds being transferred to another account, or purchases being made with their credentials.

If a user with higher privileges, such as an administrative account, is successfully targeted, a CSRF may result in a full-blown system compromise. This is because such an account can submit requests for a different order.



## **Are Cross-Site Request Forgery and Cross-Site Scripting the same?**

**CSRF and XSS are different types of attacks**, though they can be used in concert. Both of them are common JavaScript vulnerabilities.

For CSRF to work, the user must currently authenticate in an application through which the attacker can send a request. It is considered a ” one-way ” attack because requests can only be shipped with CSRF but not received; it is considered a “one-way” attack. This attack exploits an application or website’s trust for the user.

On the other hand, XSS does not require authentication but only for the user to visit a particular website on which the XSS script is then executed within the user’s browser. Because it allows for requests to be sent and received, so it is considered a “two-way” attack or vulnerability. This attack exploits the trust that a user has in the website.

### **Mitigating Cross-Site Request Forgery**

Here are few ways to protect against Cross-Site Request Forgery (CSRF) attacks:

1. Implement a strong authentication process for all users.
2. Use anti-CSRF tokens to validate requests.
3. Restrict access to sensitive data and functions.
4. Use CAPTCHA to prevent automated requests.
5. Set a maximum lifetime for sessions.
6. Use HTTPS across all pages, including login pages.
7. Enforce strong passwords and two-factor authentication.
