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

1. Broken Access Control
Broken access control occurs when access control checks are not properly enforced, allowing unauthorized access to sensitive information or system resources. This can happen due to poor implementation, weak passwords, or lack of proper security protocols. To prevent broken access control, companies and organizations should implement strong security protocols, use robust authentication methods, and regularly monitor and maintain access control measures. Examples of common access control vulnerabilities include violation of the principle of least privilege, bypassing access control checks, permitting unauthorized access to accounts, and accessing APIs without proper access controls. Preventative measures include denying access by default, reusing access control mechanisms throughout the application, enforcing record ownership, and implementing functional access control tests.

2. Cryptographic Failures
Cryptographic failures occur when cryptography is not properly implemented or used, leading to the exposure of sensitive data. This can happen due to the use of weak or outdated algorithms and protocols, poor key management, and other factors. To prevent cryptographic failures, companies and organizations should classify sensitive data and encrypt it at rest and in transit, use strong and up-to-date algorithms and protocols, and properly manage keys. Examples of common cryptographic vulnerabilities include the use of hard-coded passwords, broken or risky cryptographic algorithms, and insufficient entropy. Preventative measures include data classification, encryption, disabling caching for sensitive data, and proper key management.

3. Injection
Injection occurs when user-supplied data is not properly validated or sanitized, allowing attackers to insert malicious code into applications. This can lead to the exposure of sensitive information, data tampering, and other harmful effects. To prevent injection, organizations should use safe APIs, validate input, and properly escape special characters in dynamic queries. Examples of common injection vulnerabilities include cross-site scripting and SQL injection. Preventative measures include input validation, the use of safe APIs, and proper escaping of special characters.

4. Insecure Design
The "Insecure Design" category of the CWE Top 25 is a list of common software vulnerabilities related to design and architectural flaws. These vulnerabilities can arise when software lacks business risk profiling, has inadequate requirements and resource management, and lacks a secure design and development lifecycle. To prevent these vulnerabilities, it is recommended to establish and use a secure development lifecycle with AppSec professionals, use secure design patterns and threat modeling, integrate security language and controls into user stories, and write unit and integration tests to validate critical security controls. It is also important to implement and review security requirements, identify and mitigate security risks, and review and validate the application's design.

5. Security Misconfiguration
Misconfiguration is a security risk that occurs when an application or system is not properly configured, resulting in vulnerabilities that can be exploited by attackers. This can include issues such as having unnecessary features enabled or installed, using default accounts and passwords, and revealing overly informative error messages to users. Misconfigurations can also occur when security settings in the application stack are not set to secure values, or when security directives are not sent to clients. Misconfigurations can be prevented by implementing a repeatable hardening process and regularly reviewing and updating configurations and settings.

6. Vulnerable and Outdated Components
Vulnerable components can leave an organization open to attacks and data breaches. It is important to regularly scan for vulnerabilities and subscribe to security bulletins related to the components used in the organization. It is also important to fix or upgrade underlying platforms, frameworks, and dependencies in a timely fashion and to only obtain components from official sources over secure links. A patch management process should be in place to ensure ongoing monitoring, triaging, and applying updates or configuration changes.

7. Identification and Authentication Failures
The "Improper Authentication" category of the CWE Top 25 is a list of common software vulnerabilities related to identification failures. These vulnerabilities can be exploited through automated attacks, weak passwords, and inadequate session management. To prevent these vulnerabilities, it is recommended to implement multi-factor authentication, use strong passwords, and employ secure session management techniques. This includes using a server-side session manager that generates a new random session ID after login, and invalidating session IDs after logout, idle time, and absolute timeouts.

8. Software and Data Integrity Failures
The "Insecure Interaction Between Components" category of the CWE Top 25 is a list of common software vulnerabilities related to the integrity of code and data. These vulnerabilities can arise when an application relies on untrusted sources for plugins, libraries, or modules, or when an insecure Continuous Integration/Continuous Deployment (CI/CD) pipeline introduces the potential for unauthorized access or system compromise. To prevent these vulnerabilities, it is recommended to use digital signatures or similar mechanisms to verify the integrity of software and data, ensure that libraries and dependencies are from trusted sources, and implement a review process for code and configuration changes. It is also important to ensure the security of the CI/CD pipeline and to avoid sending unsigned or unencrypted serialized data to untrusted clients.

9. Security Logging and Monitoring Failures
The "Insufficient Logging and Monitoring" category of the CWE Top 25 is a list of common software vulnerabilities related to the detection and response to active breaches. Without proper logging and monitoring, breaches may go undetected. These vulnerabilities can arise when auditable events are not logged, log messages are inadequate or unclear, logs are not monitored for suspicious activity, and appropriate alerting and response processes are not in place. To prevent these vulnerabilities, it is recommended to ensure that all login and access control failures are logged with sufficient user context, that logs are generated in a format that log management solutions can easily consume, and that high-value transactions have an audit trail with integrity controls. It is also important to establish effective monitoring and alerting, and to have an incident response and recovery plan in place.

10. Server-Side Request Forgery (SSRF)
Server-side Request Forgery (SSRF) is a web application vulnerability that allows an attacker to send crafted requests from the server to an unexpected destination. This can happen when an application fetches a remote resource without validating the user-supplied URL. Without proper validation, an attacker can coerce the application to send a request to an unexpected destination, even if it is protected by a firewall or network access control list (ACL). SSRF attacks are becoming more common as modern web applications provide more convenient features that require fetching URLs. The severity of these attacks is also increasing due to the complexity of cloud architectures. To prevent SSRF attacks, developers should implement defense in depth controls to sanitize and validate input data, enforce URL schema and destination with a positive allow list, disable HTTP redirects, and be aware of URL consistency. It is also important to use network segmentation and "deny by default" firewall policies to block all but essential intranet traffic. Log all network flows and use network encryption for frontends with dedicated and manageable user groups.

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
[Source](https://owasp.org/www-community/Broken_Access_Control)

### 2. How brute force attacks can be used to break access control
A brute force attack is a method used by hackers to gain unauthorized access to a system, network, or application by trying a large number of possible passwords or other authentication credentials. This can be a time-consuming process, but it is effective because many people use weak passwords that can be easily guessed. To prevent brute force attacks from breaking access control, it is important to use long and complex passwords and to implement other security measures, such as two-factor authentication.
[Source](https://owasp.org/www-community/controls/Blocking_Brute_Force_Attacks)

### 3. The role of vulnerability exploitation in breaking access control
Vulnerability exploitation is a common method used by hackers to gain unauthorized access to a system, network, or application. Hackers can use known vulnerabilities in a system or application to gain access to sensitive information or to take control of the system. To prevent this from happening, it is important for companies and organizations to regularly update their systems and applications to fix any known vulnerabilities. This can help to prevent access control from being broken through vulnerability exploitation.
[Source](https://owasp.org/Top10/A01_2021-Broken_Access_Control/)

### 4. Best practices for implementing strong access control measures
To prevent access control from being broken, it is important to implement strong security protocols and to use robust authentication methods. This can include the use of long and complex passwords, as well as two-factor authentication, which requires users to provide additional information, such as a code sent to their phone, in order to access the system. It is also important to regularly monitor access to systems and applications, and to promptly investigate and address any suspicious activity. By following these best practices, companies and organizations can protect themselves from the potential damage caused by broken access control.
[Source](https://owasp.org/www-community/Access_Control)

### 5. The importance of regular monitoring and maintenance for preventing broken access control.
Regular monitoring and maintenance of access control measures is important for preventing them from being broken. By regularly checking for and addressing any potential vulnerabilities, companies and organizations can ensure that their access control measures remain effective. This can help to prevent security breaches and protect sensitive information. Additionally, prompt investigation and response to any suspicious activity can help to prevent access control from being broken and can minimize the potential damage caused by a breach.
[Source](https://owasp.org/www-community/Broken_Access_Control)

## DOT Framework matrix
| Research part | Library | Field | Lab | Showroom | Workshop |
|:------------|:---|:---|:---|:---|:---:|
| What is OWASP? | x | | | | |
| How does OWASP work? | x | | | | |
| When do I need OWASP | x | | | | |
| What are the dangers of not using OWASP? | x | | | | |
| How to use OWASP? | x | | | | |
| Proof of concept | | | | | x |
| Research: How to implement OWASP in the Happilly project? | | | | x | |
