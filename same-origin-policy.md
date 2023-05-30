# Same Origin Policy

<figure><img src=".gitbook/assets/image (8).png" alt="" width="314"><figcaption></figcaption></figure>



The Same Origin Policy (SOP) is an important security mechanism that enforces a browser's restrictions on scripts from different origins. This policy prevents malicious scripts from one domain from accessing data from a different domain.

For example, a malicious script on a website in domain A would not be able to access sensitive data from domain B. This policy is also enforced for external scripts, such as JavaScript from a third-party provider.

In addition, the Same Origin Policy can also be used to protect against Cross-Site Request Forgery (CSRF) attacks. With CSRF, an attacker can force a user's browser to send an unwanted or malicious request to a server. By enforcing the Same Origin Policy, these malicious requests can be blocked.

The Same Origin Policy can be implemented in a few different ways. One way is to use a web application firewall (WAF) which can be configured to enforce the Same Origin Policy. This ensures that requests from different domains are blocked.

Another way to enforce the Same Origin Policy is by using a Content Security Policy (CSP). CSP is a security policy which can be used to specify which domains are allowed to access a given resource. With CSP, it's possible to specify which domains are allowed to access a given resource, and therefore enforce the Same Origin Policy.

Apache web server provides the capability to control access to resources based on the same origin policy by using the **mod\_rewrite** module. To enforce the SOP, the `mod_rewrite` module can be used to specify which requests should be allowed and which should be denied.

Another example is the [NGINX web server](https://nginx.org/). With NGINX, the same origin policy can be implemented by using the [limit\_req](https://nginx.org/en/docs/http/ngx\_http\_limit\_req\_module.html) module. This module allows administrators to specify a limit on the number of requests that can be made from a given origin.

Finally, the [IIS web server](https://www.iis.net/) provides the capability to control access to resources based on the same origin policy by using the [Request Filtering](https://docs.microsoft.com/en-us/iis/configuration/system.webserver/security/requestfiltering/) feature. This feature allows administrators to specify which requests should be allowed and which should be denied.

By implementing the same origin policy on web servers, administrators can ensure that only requests from the same origin are allowed, thus reducing the risk of malicious cross-site scripting attacks.



## References <a href="#22a2" id="22a2"></a>

* [https://developer.mozilla.org/en-US/docs/Web/Security/Same-origin\_policy](https://developer.mozilla.org/en-US/docs/Web/Security/Same-origin\_policy)
* [https://portswigger.net/web-security/cors/same-origin-policy](https://portswigger.net/web-security/cors/same-origin-policy)
* [https://web.dev/same-origin-policy/](https://web.dev/same-origin-policy/)
