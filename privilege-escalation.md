# Privilege Escalation

<figure><img src=".gitbook/assets/image (17).png" alt="" width="314"><figcaption></figcaption></figure>

### **Privilege Escalation**

Privilege escalation is the process of exploiting a system vulnerability to gain higher-level permissions for an existing user account. This could be done by exploiting a bug in the system, using a back door, or by exploiting the administrator’s weak password.

### Story **of Privilege Escalation**

The concept of privilege escalation has been around since the early days of computing, with the first recorded instance occurring in the 1970s. Since then, the techniques used to exploit systems for privilege escalation have become more sophisticated.

In the 1980s, the concept of “ring protection” was developed. This was a system of privilege rings that was used to limit the amount of access a user had to resources and data on a computer system. This system was used to prevent users from accessing resources they were not authorized to access.

In the 1990s, the concept of “mandatory access control” was developed. This system was used to restrict access to sensitive information, such as financial data, by assigning levels of access to different users. This system was used to further limit the amount of access a user had to resources on a computer system.

Since then, the concept of privilege escalation has been further refined and is now used to protect computer systems from malicious users and attackers. With the rise of the Internet and the development of more powerful computers, the techniques used to exploit systems for privilege escalation have become more sophisticated.

Privilege escalation can be classified into two main types: vertical privilege escalation and horizontal privilege escalation.

### **Vertical Privilege Escalation**

Vertical privilege escalation occurs when a user with limited privileges is able to access higher privileges than they are normally allowed. The most common example of this is when an unprivileged user is able to access administrator-level privileges. This can be accomplished by exploiting a vulnerability in the system, using a back door, or by exploiting the administrator’s weak password.

Vertical privilege escalation can be accomplished in a number of ways, including using commands. For example, a user can use the `sudo` command to gain higher privileges on a Linux system. On a Windows system, a user can use the `runas` command to run a program with a different user's credentials. Additionally, on both Linux and Windows systems, a user can use the `su` command to switch to a different user and gain their privileges.

### **Horizontal Privilege Escalation**

Horizontal privilege escalation occurs when a user with one set of privileges is able to access another user’s privileges. The most common example of this is when an unprivileged user is able to access a privileged user’s files or data.

Horizontal privilege escalation can be accomplished in a number of ways, such as exploiting a vulnerability in the system, using a back door, or by exploiting the privileged user’s weak password. In addition, there are a number of commands that can be used to gain access to the privileged user’s data.

On a Linux system, a user can use the `find` command to search for a specific file or directory. Additionally, a user can use the `su` command to switch to a different user and gain their privileges. On a Windows system, a user can use the `runas` command to run a program with a different user's credentials, or they can use the `net` command to list all the users on the system and their associated privileges.

### **Mitigation of Privilege Escalation**

There are several steps that can be taken to mitigate the risks associated with privilege escalation.

1. Implement strong authentication and authorization protocols. Access to sensitive data should be restricted to users with the appropriate privileges.
2. Ensure that the system is regularly updated with the latest security patches. This will help to prevent attackers from exploiting vulnerabilities in the system.
3. Restrict physical access to the system. This will prevent attackers from using physical means to gain access to the system.
4. Use just in time access for systems that are required to log in less frequently.

### **Additional Resources**

For more information about privilege escalation for Windows and Linux, the following links may be helpful:

* [Windows Privilege Escalation](https://pentest-tools.com/blog/windows-privilege-escalation/)
* [Linux Privilege Escalation](https://pentest-tools.com/blog/linux-privilege-escalation/)
