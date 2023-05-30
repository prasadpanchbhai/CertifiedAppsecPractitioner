# TLS security

<figure><img src=".gitbook/assets/image (4).png" alt="" width="314"><figcaption></figcaption></figure>

### **Defining TLS Security**

TLS security, or Transport Layer Security, is a cryptographic protocol designed to provide secure communication between two parties, typically a client and a server. TLS is used to secure communication between a user's browser and a web server, and also to secure other types of communication such as email, file transfers, and virtual private networks (VPNs).

TLS security is composed of two main types, TLS 1.2 and TLS 1.3. TLS 1.2 is the most widely used version, and is the default for most web browsers, but TLS 1.3 is gradually becoming more popular as it is more secure.

### **TLS 1.0 and 1.1**

TLS 1.0 and 1.1 were the first versions of TLS security, and were released in 1999 and 2006, respectively. While TLS 1.0 and 1.1 can still be used to secure communication between two parties, they are considered less secure than TLS 1.2 and 1.3.

TLS 1.0 and 1.1 use symmetric encryption to secure the connection, meaning that the same key is used to encrypt and decrypt the data. This makes them vulnerable to certain attacks, such as man-in-the-middle attacks, where the attacker can intercept the communication and access the data. Additionally, TLS 1.0 and 1.1 do not support modern authentication protocols such as Elliptic Curve Cryptography, making them vulnerable to remote code execution attacks.

For these reasons, it is strongly recommended to use TLS 1.2 or TLS 1.3 for secure communication, as they are more secure and support modern authentication protocols.

### **TLS 1.2**

TLS 1.2 is the most widely used version of TLS security. It was first released in 2008, and is used to secure communication between two parties using a combination of encryption, authentication, and data integrity.

TLS 1.2 uses symmetric encryption to secure the connection, meaning that the same key is used to encrypt and decrypt the data. It also uses authentication to ensure that the two parties involved in the communication are who they say they are, and data integrity to ensure that the data has not been modified in transit.

An example of TLS 1.2 in action would be a user's web browser connecting to a secure website. The browser will use TLS 1.2 to encrypt the connection, verify the identity of the website, and ensure that the data has not been modified in transit.

### **TLS 1.3**

TLS 1.3 is the newest version of TLS security, and is gradually becoming more popular as it is more secure than TLS 1.2. It was first released in 2018, and is used to secure communication between two parties using a combination of encryption, authentication, and data integrity.

TLS 1.3 uses asymmetric encryption to secure the connection, meaning that two different keys are used to encrypt and decrypt the data. It also uses authentication to ensure that the two parties involved in the communication are who they say they are, and data integrity to ensure that the data has not been modified in transit.

An example of TLS 1.3 in action would be a user's web browser connecting to a secure website. The browser will use TLS 1.3 to encrypt the connection, verify the identity of the website, and ensure that the data has not been modified in transit. Additionally, TLS 1.3 is more secure than TLS 1.2, as it uses a combination of encryption, authentication, and data integrity to protect the connection.
