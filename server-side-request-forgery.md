# Server-Side Request Forgery

<figure><img src=".gitbook/assets/image (15).png" alt="" width="314"><figcaption></figcaption></figure>

### **Server-Side Request Forgery (SSRF)**

Server-Side Request Forgery (SSRF) is an attack method that enables an attacker to send requests from a vulnerable web application to internal or external systems. It can be used to bypass access controls or to access confidential data.

### **History of SSRF Attacks**

Server-Side Request Forgery (SSRF) has existed since the early 2000s, and has been used in various types of attacks, from data exfiltration to system exploitation. It has been a major security concern for organizations, as it can be used to bypass access controls and access sensitive information.

In 2006, researchers discovered a critical vulnerability in Microsoft IIS which allowed attackers to use SSRF to send requests to arbitrary hosts on the internet. This vulnerability was used in a series of attacks, including an attack on the RockYou social networking site which compromised 32 million user accounts.

In 2008, researchers discovered a critical vulnerability in Microsoft Exchange which allowed attackers to use SSRF to access internal systems. This vulnerability was used in the Aurora attack, which targeted Google and over 20 other organizations.

In 2010, a zero-day vulnerability in Microsoft Internet Explorer was discovered which allowed attackers to use SSRF to access internal systems. This vulnerability was used in a series of targeted attacks, dubbed Operation Aurora.

SSRF attacks have continued to be a threat to organizations, as attackers have become more adept at exploiting them. Organizations should remain vigilant and take steps to protect themselves from these attacks.

### **Types of SSRF**

SSRF attacks can be classified into two types:

1. **External SSRF** - This type of attack is used to target external networks. It can be used to access services that are not exposed to the public, such as internal network resources or services on private or restricted networks.
2. **Internal SSRF** - This type of attack is used to target internal systems. It can be used to access internal services, such as databases or file systems, or to access sensitive information such as user data or system configuration files.

### **Examples of SSRF**

Some examples of SSRF attacks are:

1. **Scanning internal networks** - An attacker can use SSRF to scan internal networks, allowing them to discover and exploit vulnerable internal systems.
2. **Bypassing firewalls** - SSRF can be used to bypass firewall rules by sending malicious requests directly to internal systems.
3. **Reading files** - An attacker can use SSRF to read sensitive information from internal systems, such as user data or system configuration files.
4. **Executing code** - An attacker can use SSRF to execute malicious code on internal systems.



### HOW IT WORKS

For example :-&#x20;

GET /?url=http://google.com/ HTTP/1.1&#x20;

Host: [example.com](http://example.com/).&#x20;

Here [example.com](http://example.com/) fetch [http://google.com](http://google.com) from its server.

1. Attacker Sends the Request the [Example.com](http://example.com/) (Which is the Vulnerable Application) server to fetch the request from “[google.com](http://google.com/)”.
2. Now [Example.com](http://example.com/)'s server is vulnerable to SSRF attack so it will fetch the response of [google.com](http://google.com/) request.
3. Send a response back to the Attackers.



### **IMPACT OF SSRF ATTACKS**

If an attacker is able to control the destination of the server side requests they can potentially perform the following actions:-

* Bypass IP whitelisting.
* Bypass host-based authentication services.
* Read files from the web server.
* Retrieve sensitive information such as the IP address of the web server behind a reverse proxy.
* Port Scans or Cross Site Port Attack.
* Server Side Rendering.
* Sensitive data exposure.
* Scan the internal network to which the server is connected to.



### Remediation

* Implement input validation.
* Use Regular Expressions (RegEx).
* Only accept the intended IP address format (IPv4 or IPv6).
* To compare against the allow list, use the method/output library’s value as the IP address.
* Validate incoming Domain Names.
