---
description: Certified Appsec Practitioner (CAP) — Study Notes Pt.2
---

# Whitelisting & Blacklisting

<figure><img src=".gitbook/assets/image (2) (1).png" alt="" width="314"><figcaption></figcaption></figure>

### **Blacklisting**&#x20;

**Blacklisting** is the practice of only rejecting input that is known to be bad. This commonly involves rejecting input that contains content that is specifically known to be malicious by looking through the content for a number of “known bad” characters, strings, or patterns. This approach is generally weaker than whitelist validation because the list of potentially bad characters is extremely large, and as such any list of bad content is likely to be large, slow to run through, incomplete, and difficult to keep up to date.

A common method of implementing a blacklist is also to use regular expressions, with a list of characters or strings to disallow, such as the following example:

_`‘|%| — |;|/\|\\\||\[|@|xp`_

In general, you should not use blacklisting in isolation, and you should use whitelisting if possible. However, in scenarios where you cannot use whitelisting, blacklisting can still provide a useful partial control. In these scenarios, however, it is recommended that you use blacklisting in conjunction with output encoding to ensure that input passed elsewhere (e.g., to the database) is subject to an additional check to ensure that it is correctly handled to prevent SQL injection.

**Damage & Defense…**

* _**Blacklisting**_ or _blacklist validation_ attempts to check that given data does not contain “known bad” content. For example, a web application may block input that contains the exact text `<SCRIPT>` in order to help prevent XSS. However, this defense could be evaded with a lower case script tag or a script tag of mixed case.



### Whitelisting

**Whitelist** validation is the practice of only accepting input that is known to be good. This can involve validating compliance with the expected type, length or size, numeric range, or other format standards before accepting the input for further processing.&#x20;

**For example,** validating that an input value is a credit card number may involve validating that the input value contains only numbers, is between 13 and 16 digits long, and passes the business logic check of correctly passing the Luhn formula (the formula for calculating the validity of a number based on the last “check” digit of the card).

When using whitelist validation you should consider the following points:

* **Data type** Is the data type correct? If the value is supposed to be numeric, is it numeric? If it is supposed to be a positive number, is it a negative number instead?
* **Data size** If the data is a string, is it of the correct length? Is it less than the expected maximum length? If it is a binary blob, is it less than the maximum expected size? If it is numeric, is it of the correct size or accuracy? (For example, if an integer is expected, is the number that is passed too large to be an integer value?)
* **Data range** If the data is numeric, is it in the expected numeric range for this type of data?
* **Data content** Does the data look like the expected type of data? For example, does it satisfy the expected properties of a ZIP Code if it is supposed to be a ZIP Code? Does it contain only the expected character set for the data type expected? If a name value is submitted, only some punctuation (single quotes and character accents) would normally be expected, and other characters, such as the less than sign (<), would not be expected.

A common method of implementing content validation is to use regular expressions. Following is a simple example of a regular expression for validating a U.S. ZIP Code contained in a string:

> _**^\d{5}(-\d{4})?$**_

In this case, the regular expression matches both five-digit and five-digit + four-digit ZIP Codes as follows:

▪\*\*\*^\d{5}\*\*\* Match exactly five numeric digits at the start of the string.▪\*\*\*(–\d{4})?\*\*\* Match the dash character plus exactly four digits either once (present) or not at all (not present).▪$ This would appear at the end of the string. If there is additional content at the end of the string, the regular expression will not match.

In general, **whitelist validation** is the more powerful of the two input validation approaches. It can, however, be difficult to implement in scenarios where there is complex input, or where the full set of possible inputs cannot be easily determined. Difficult examples may include applications that are localized in languages with large character sets (e.g., Unicode character sets such as the various Chinese and Japanese character sets). It is recommended that you use whitelist validation wherever possible, and then supplement it by using other controls such as output encoding to ensure that information that is then submitted elsewhere (such as to the database) is handled correctly.



## Designing an Input Validation and Handling Strategy <a href="#82d6" id="82d6"></a>

Input validation is a valuable tool for securing an application. However, it should be only part of a defense-in-depth strategy, with multiple layers of defense contributing to the application’s overall security. Here is an example of an input validation and handling strategy utilizing some of the solutions presented in this chapter:

* Whitelist input validation used at the application input layer to validate all user input as it is accepted by the application. The application allows only input that is in the expected form.
* Whitelist input validation also performed at the client’s browser. This is done to avoid a round trip to the server in case the user enters data that is unacceptable. You cannot rely on this as a security control, as all data from the user’s browser can be altered by an attacker.
* Blacklist and whitelist input validation present at a Web application firewall (WAF) layer (in the form of vulnerability “signatures” and “learned” behavior) to provide intrusion detection/prevention capabilities and monitoring of application attacks.
* Parameterized statements used throughout the application to ensure that safe SQL execution is performed.
* Encoding used within the database to safely encode input when used in dynamic SQL.
* Data extracted from the database appropriately encoded before it is used. For example, data being displayed in the browser is encoded for cross-site scripting (XSS).
