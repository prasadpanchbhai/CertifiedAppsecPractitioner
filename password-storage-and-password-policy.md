# Password Storage and Password Policy

<figure><img src=".gitbook/assets/image (2).png" alt="" width="314"><figcaption></figcaption></figure>



### **Password Storage and Password Policy**

Password storage and password policy are two important aspects of information security. Password storage refers to the practice of securely storing passwords so that they are not accessible to unauthorized individuals. This can be done through various methods, such as encryption, hashing, and salting.

Password policy, on the other hand, is a set of rules that dictates how users should create, store, and manage their passwords. These rules may include the length and complexity of passwords, the frequency of password changes, and the use of two-factor authentication. By following a strong password policy, organizations can help ensure that their users' passwords remain secure.

#### **Password Storage**

Password storage can be done through a variety of methods. For instance, encryption is a method that encodes data so that it is unreadable to unauthorized individuals. Hashing is another method that transforms a password into a unique string of characters. Salting is a technique that adds an extra layer of security, as it combines a password with a random string of characters.

To securely store these passwords, organizations should use strong encryption algorithms, such as AES and RSA. Additionally, passwords should be stored in a secure location, such as a password manager or a secure database. Organizations should also ensure that passwords are not stored in plain text or shared with unauthorized individuals.

When storing passwords, organizations should not use plain text or share them with unauthorized individuals. Additionally, passwords should not be stored on physical documents or in unsecured locations, such as on computers that are connected to the internet. Organizations should also ensure that any passwords sent via email or other forms of communication are encrypted.

#### **Password Policy**

Password policy is an important aspect of information security. By following a strong password policy, organizations can help ensure that their users' passwords remain secure. Password policies are dependent on organizations and the type of work they do. Some of the password policies that could be set are as follows:

1. Passwords should be at least 12 characters in length.
2. Passwords should contain a mix of lowercase and uppercase letters, numbers, and special characters.
3. Passwords should not contain easily guessable words or phrases.
4. Passwords should be changed at least every 90 days.
5. Passwords should not be reused.
6. Passwords should not be shared with unauthorized individuals.
7. Passwords should not be stored in plain text.
8. Passwords should not be stored in unsecured locations.
9. Passwords should be encrypted when sent via email or other communication methods.
10. Organizations should utilize two-factor authentication when possible.



This cheat sheet provides guidance on the various areas that need to be considered related to storing passwords. In short:

* Use **Argon2id** with a minimum configuration of 19 MiB of memory, an iteration count of 2, and 1 degree of parallelism.
* If **Argon2id** is not available, use **scrypt** with a minimum CPU/memory cost parameter of (2^17), a minimum block size of 8 (1024 bytes), and a parallelization parameter of 1.
* For legacy systems using **bcrypt**, use a work factor of 10 or more and with a password limit of 72 bytes.
* If FIPS-140 compliance is required, use **PBKDF2** with a work factor of 600,000 or more and set with an internal hash function of HMAC-SHA-256.
* Consider using a **pepper** to provide additional defense in depth (though alone, it provides no additional secure characteristics).
