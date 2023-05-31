# Insecure File Uploads

<figure><img src=".gitbook/assets/image (18).png" alt="" width="314"><figcaption></figcaption></figure>



### **Insecure File Uploads**

File upload vulnerability is a common security issue found in web applications. Whenever the web server accepts a file without validating it or keeping any restriction, it is considered as an unrestricted file upload.

### **Types of Insecure File Uploads**

There are several types of insecure file uploads, including:

* Unrestricted File Upload
* Insecure File Extensions
* Insecure Storage
* Unvalidated File Contents

### **Unrestricted File Upload**

Unrestricted file upload is a vulnerability that allows an attacker to upload malicious files to a web application. This can be done by exploiting the lack of authentication or authorization checks on the server-side of the application. Examples of this attack include uploading a malicious script or executable to a vulnerable web application.

### **Insecure File Extensions**

Insecure file extensions are file types that are vulnerable to attack. These include .exe, .vbs, .php and other types of scripts and executables. By allowing these types of files to be uploaded to a web application, the attacker can gain access to the application and its data.

### **Insecure Storage**

Insecure storage is where files uploaded to a web application are stored in an insecure location. For example, an attacker could upload a malicious file to a web application and then access the file from an insecure location.

### **Unvalidated File Contents**

Unvalidated file contents is a vulnerability where an attacker can upload a malicious file to a web application. This can be done by exploiting the lack of authentication or authorization checks on the server-side of the application. Examples of this attack include uploading a malicious script or executable to a vulnerable web application. These files can then be used to gain access to the application and its data.

### **Examples of Code Requests and Responses**

The following example code shows an insecure file upload request and response:

Request:

```
POST /upload.php HTTP/1.1
Host: example.com
Content-Type: multipart/form-data; boundary=----WebKitFormBoundary7MA4YWxkTrZu0gW

------WebKitFormBoundary7MA4YWxkTrZu0gW
Content-Disposition: form-data; name="uploaded_file"; filename="example.php"
Content-Type: application/x-php

<?php system($_GET['cmd']);?>
------WebKitFormBoundary7MA4YWxkTrZu0gW--

```

Response:

```
HTTP/1.1 200 OK
Content-Type: text/html; charset=utf-8

File uploaded successfully!

```

### **Real-Life Examples**

Real-life examples of insecure file uploads can include:

* Malicious files uploaded to a website, such as a PHP shell
* Unsecured files being uploaded to a server
* Unvalidated files being uploaded to a database

### **Mitigating Insecure File Uploads**

Insecure file uploads can be mitigated by following these steps:

1. Perform authentication and authorization checks on the server-side of the application.
2. Restrict the types of files that can be uploaded to the web application.
3. Validate that the uploaded file is of the expected type.
4. Ensure that the uploaded files are stored securely.
5. Perform regular scans of the uploaded files for malicious content.
