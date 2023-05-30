# Security Headers.

<figure><img src=".gitbook/assets/image (2).png" alt="" width="314"><figcaption></figcaption></figure>



### **Security Hardening**

* Security hardening is the process of enhancing system security through the use of a variety of security measures. It is an important process for any organization or individual who wants to ensure the security of their systems and data. There are a variety of security hardening techniques that can be used to improve the overall security posture of an organization.

#### **Encrypt Data at Rest**

* Encrypting data at rest is an important security best practice that helps to ensure that only authorized users can access, modify, or delete data. Encryption can be used to protect data stored on a variety of storage media, including hard drives, USB drives, and cloud storage. When using encryption, it is important to use strong encryption algorithms and keys to ensure that data is properly protected.

#### **Enforce Strong Passwords**

* Having strong passwords is essential to protecting an organization's systems and data. All accounts should have strong passwords, with a minimum of eight characters, including upper and lowercase letters, numbers, and special characters. Additionally, passwords should be changed regularly, and users should not share or reuse passwords for multiple accounts.

#### **Restrict Access to Sensitive Data**

* Restricting access to sensitive data is an important security best practice. Access to sensitive data should be limited to only those users who need it to perform their roles. This helps to ensure that only those with the necessary permissions can access the data, reducing the risk of it being accessed by unauthorized users.

#### **Use Two-Factor Authentication**

* Two-factor authentication (2FA) is an important security measure that helps to ensure that only users with the correct credentials can access the system. 2FA requires users to enter two pieces of information to gain access to a system, such as a username and a password, or a username and a code sent to a mobile device. This helps to ensure that only the correct user can gain access to the system.

#### **Patch Regularly**

* Security patches are an important part of keeping a system secure. Installing security patches regularly helps to ensure that the system is up-to-date and secure. Security patches can help to protect against known vulnerabilities, as well as any new vulnerabilities that may have been discovered since the last patch was installed.

#### **Monitor System Activity**

* Monitoring system activity is an important security best practice. Monitoring system activity can help to identify potential security threats and take action to mitigate them. It can also help to identify any unauthorized access attempts, allowing administrators to take action to prevent any further attempts.
* Security hardening is an important process for any organization or individual who wants to ensure the security of their systems and data. By using a variety of security hardening techniques, organizations can help to ensure that their systems and data remain secure. This can help to protect against malicious actors, as well as any potential vulnerabilities in the system.



### **Security Headers**

Security headers are HTTP response headers that help protect web applications from malicious attacks. They provide a layer of defense against Cross-Site Scripting (XSS) attacks, clickjacking, and cross-site information leakage. Security headers can also be used to limit the sources from which resources can be loaded and to control the Referer header sent in requests. Implementing security headers is an important part of any secure web application and can help mitigate the risk of malicious attacks.

#### **Content-Security-Policy**

* Content-Security-Policy (CSP) is a response header that helps protect against XSS attacks. It allows you to specify the sources from which your application is allowed to load resources, such as scripts, images, and style sheets.
*   For example, you can use the following CSP to restrict the browser from executing any script from outside your domain:

    `Content-Security-Policy: default-src 'self'; script-src 'self'`

#### **X-XSS-Protection**

* X-XSS-Protection is a response header that helps protect against XSS attacks by enabling the browser's built-in XSS protection.
*   For example, the following X-XSS-Protection header will enable the browser's XSS protection and also report any violations of the policy to the specified URL:

    `X-XSS-Protection: 1; report=<https://example.com/xss-report>`

#### **X-Frame-Options**

* X-Frame-Options is a response header that is used to protect against clickjacking attacks by preventing the page from being embedded in a frame. It can be used to restrict which web servers can embed the page in a frame.
*   For example, the `DENY` directive can be used to prevent any web server from embedding the page in a frame:

    `X-Frame-Options: DENY`
*   The `SAMEORIGIN` directive can be used to restrict embedding to web servers that are on the same origin as the page:

    `X-Frame-Options: SAMEORIGIN`

#### **Referrer-Policy**

* Referrer-Policy is a response header that is used to control the Referer header sent in requests. It can be used to protect against cross-site information leakage by limiting the amount of information sent in the Referer header.
* There are several directives that can be used with `Referrer-Policy`. The no-referrer directive can be used to prevent any Referer header from being sent in requests. This directive is useful for preventing cross-site information leakage.
