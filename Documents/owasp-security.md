# Security research
## Table of contents
- [1. What is OWASP](#1-what-is-owasp)
- [2. What is the OWASP Top 10](#2-what-is-the-owasp-top-10)
- [3. Broken Access Control](#3-broken-access-control)
- [4. Sub topics about Broken Access Control](#4-broken-access-control-sub-topics)

## 1. What is OWASP
OWASP, or the Open Web Application Security Project, is a nonprofit organization that focuses on improving the security of software. It provides resources like the OWASP Top 10, a list of common web application security vulnerabilities, and local chapters for security professionals to connect and share knowledge. It is a valuable resource for developers, security professionals, and organizations looking to secure their web applications.

## 2. What is the OWASP Top 10
The OWASP Top 10 is a list of the most critical web application security risks, as determined by a global community of experts. Here is a short summary of the OWASP Top 10:

1. Injection attacks: 
Injection attacks occur when malicious data is inserted into a database or other system via user input.

2. Broken authentication and session management: 
This refers to weaknesses in the way authentication and session management is implemented, which can allow attackers to gain access to sensitive data.

3. Cross-site scripting (XSS): 
XSS attacks involve injecting malicious code into a website, which is then executed by users who visit the site.

4. Insecure direct object references: 
This refers to a weakness in the way applications handle references to objects, such as files or database records, which can be exploited by attackers to gain access to sensitive data.

5. Security misconfiguration: 
This refers to the incorrect configuration of security settings on a system, which can leave it vulnerable to attack.

6. Sensitive data exposure: 
This refers to the improper storage or transmission of sensitive data, such as passwords or credit card numbers, which can lead to data breaches.

7. Cross-site request forgery (CSRF): 
CSRF attacks involve tricking users into making unauthorized requests to a website, such as changing their password or transferring funds.

8. Using components with known vulnerabilities: 
This refers to the use of third-party components, such as libraries or frameworks, that have known vulnerabilities, which can leave an application open to attack.

9. Failure to restrict URL access: 
This refers to the failure to properly restrict access to sensitive pages or URLs within an application, which can allow attackers to gain unauthorized access.

10. Insufficient transport layer protection: 
This refers to the failure to properly encrypt data when it is transmitted over the network, which can allow attackers to intercept and read sensitive data.

[Source](https://owasp.org/www-project-top-ten/)

## 3. Broken Access Control
Access control is a security measure that controls who has access to a system, network, or application. It is an important aspect of computer security and is used to prevent unauthorized access to sensitive information.

However, access control can be broken, which can lead to serious security breaches. This can happen for a variety of reasons, such as poor implementation, weak passwords, or lack of proper security protocols.

One common way that access control can be broken is through the use of brute force attacks. In a brute force attack, a hacker uses automated software to try a large number of possible passwords or other authentication credentials until the correct one is found. This can be a time-consuming process, but it is effective because many people use weak passwords that can be easily guessed.

Another way that access control can be broken is through the exploitation of vulnerabilities in the system or application. Hackers can use these vulnerabilities to gain access to sensitive information or to take control of the system. This is why it is important for companies and organizations to regularly update their systems and applications to fix any known vulnerabilities.

In order to prevent access control from being broken, it is important to implement strong security protocols and to use robust authentication methods. This can include the use of long and complex passwords, as well as two-factor authentication, which requires users to provide additional information, such as a code sent to their phone, in order to access the system.

It is also important to regularly monitor access to systems and applications, and to promptly investigate and address any suspicious activity. By taking these steps, companies and organizations can protect themselves from the potential damage caused by broken access control.
[Source](https://medium.com/purplebox/broken-access-control-f82235ddf888) 

## 4. Broken Access Control Sub topics
### 1. The risks and consequences of broken access control
Broken access control can lead to serious security breaches and can have significant consequences for individuals and organizations. It can result in the loss of sensitive information, financial losses, and damage to a company's reputation. To prevent broken access control, it is important to implement strong security protocols and to regularly monitor and maintain access control measures.

### 2. How brute force attacks can be used to break access control
A brute force attack is a method used by hackers to gain unauthorized access to a system, network, or application by trying a large number of possible passwords or other authentication credentials. This can be a time-consuming process, but it is effective because many people use weak passwords that can be easily guessed. To prevent brute force attacks from breaking access control, it is important to use long and complex passwords and to implement other security measures, such as two-factor authentication.

### 3. The role of vulnerability exploitation in breaking access control
Vulnerability exploitation is a common method used by hackers to gain unauthorized access to a system, network, or application. Hackers can use known vulnerabilities in a system or application to gain access to sensitive information or to take control of the system. To prevent this from happening, it is important for companies and organizations to regularly update their systems and applications to fix any known vulnerabilities. This can help to prevent access control from being broken through vulnerability exploitation.

### 4. Best practices for implementing strong access control measures
To prevent access control from being broken, it is important to implement strong security protocols and to use robust authentication methods. This can include the use of long and complex passwords, as well as two-factor authentication, which requires users to provide additional information, such as a code sent to their phone, in order to access the system. It is also important to regularly monitor access to systems and applications, and to promptly investigate and address any suspicious activity. By following these best practices, companies and organizations can protect themselves from the potential damage caused by broken access control.

### 5. The importance of regular monitoring and maintenance for preventing broken access control.
Regular monitoring and maintenance of access control measures is important for preventing them from being broken. By regularly checking for and addressing any potential vulnerabilities, companies and organizations can ensure that their access control measures remain effective. This can help to prevent security breaches and protect sensitive information. Additionally, prompt investigation and response to any suspicious activity can help to prevent access control from being broken and can minimize the potential damage caused by a breach.
