# Encoding, Encryption and Hashing

<figure><img src=".gitbook/assets/image (7).png" alt="" width="314"><figcaption></figcaption></figure>

Encoding, encryption, and hashing are three distinct processes used to protect digital information.

_**Encoding**_ is a way of representing data in a different format, typically for the purpose of obfuscation or to compress the data. It does not provide security, but can be used to help make it more difficult for unauthorized persons to access the data.

_**Encryption**_ is a process of transforming data using an algorithm and a key in order to make the data unreadable without the key. It is the most commonly used method to protect data in transit and at rest.

_**Hashing**_ is the process of generating a fixed-length output from a string of data using a deterministic algorithm. It is used to verify the integrity of data and to securely store passwords.

### **Types of Encoding**

Encoding can be used for a variety of purposes, but most commonly it is used to compress data or obfuscate data from unauthorized access. There are several types of encoding commonly used, including:

* **URL Encoding**: Used to encode characters in a URL string, so the URL can be sent over the web without causing errors.
* **Base64 Encoding**: Used to convert arbitrary binary data into a string of ASCII characters.
* **ASCII Encoding**: Used to convert text into a 7-bit encoding.
* **UTF-8 Encoding**: Used to encode characters in Unicode for internationalization purposes.
* **Hexadecimal Encoding**: Used to represent binary data in a more human-readable format.

### **Types of Encryption**

Encryption is the process of transforming data using an algorithm and a key in order to make the data unreadable without the key. It is the most commonly used method to protect data in transit and at rest.

* **Symmetric Encryption**: Uses the same key for both encryption and decryption.
* **Asymmetric Encryption**: Uses two different keys, one for encryption and one for decryption.

### **Symmetric Encryption**

Symmetric encryption is a type of encryption where the same key is used for both encryption and decryption. It is relatively easy to implement and provides a high level of security.

The most common type of symmetric encryption is [AES](https://en.wikipedia.org/wiki/Advanced\_Encryption\_Standard) or Advanced Encryption Standard. This type of encryption uses a 128-bit, 192-bit, or 256-bit key to encrypt data. The longer the key, the more secure it is. Each bit is represented by a binary number, and the number of possible combinations increases exponentially with each additional bit.

To use AES, the data is divided into blocks and then each block is encrypted using the key. This process is repeated until all the data is encrypted. To decrypt the data, the same process is repeated in reverse.

### **Asymmetric Encryption**

Asymmetric encryption is a type of encryption where two different keys are used, one for encryption and one for decryption. It is more secure than symmetric encryption because the encryption and decryption keys are not the same.

The most common type of asymmetric encryption is [RSA](https://en.wikipedia.org/wiki/RSA\_\(cryptosystem\)), or Rivest–Shamir–Adleman. This type of encryption uses two keys, a public key, and a private key. The public key is used to encrypt the data, and the private key is used to decrypt the data.

To use RSA, the data is encrypted using the public key and then decrypted using the private key. This process ensures that only the intended recipient of the data can decrypt it, as they are the only ones with the private key.

### **What is Hashing?**

Hashing is the process of generating a fixed-length output from a string of data using a deterministic algorithm. It is used to verify the integrity of data and to securely store passwords.

There are several types of hashing algorithms commonly used, including:

* **MD5**: Generates a 128-bit hash value.
* **SHA-1**: Generates a 160-bit hash value.
* **SHA-2**: Generates a 224-bit, 256-bit, 384-bit, or 512-bit hash value.
* **SHA-3**: Generates a 224-bit, 256-bit, 384-bit, or 512-bit hash value.
* **BCrypt**: Generates a variable-length hash value based on a salt and user-supplied password.
