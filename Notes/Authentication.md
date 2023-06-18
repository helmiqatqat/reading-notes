# Authentication

## Securing Passwords

**Explain to a non-technical friend how you would safely hash and store a password.**

- Imagine the password some kind of jewelry, and the level of encryption is safe, so imagine we want to put this jewelry in the safe, the safe cannot be openned unless you try every key in the room you are in 'which are more than you can ever reach counting', only the safe maker knows what key is the right one for the safe and in that case the safe maker is basicly the algorithm itself.

**What is Bcrypt?**

- It is an algorithm used to encrypt data.

**Why might you use something like Bcrypt?**

- Because it is slow and strong, Hashes can't be reversed (one way ), so instead of reversing the hash of the password, an attacker can simply keep trying different inputs until he does not find the right now that generates the same hash value, called brute force attack. Using a modern computer one can crack a 16 Character Strong password in less than an hour, thanks to GPU. But what makes Bcrypt unique is it having the security factor called as work factor. This work factor value determines how slow the hash function will be, means different work factor will generate different hash values in different time span, which makes it extremely resistant to brute force attacks. When computers become faster next year we can increase the work factor to balance it out i.e. to make the attack slower.

## Basic Auth

**What is Basic Authentication?**

- Basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request.

**What properties are necessary in the header of a Basic Auth request?**

- A request contains a header field in the form of ````Authorization: Basic <credentials>````, where credentials is the Base64 encoding of ID and password joined by a single colon :.

**How are username:password in Basic Auth encoded?**

- If the browser uses ````Aladdin```` as the username and ````open sesame```` as the password, then the field's value is the Base64 encoding of ````Aladdin:open sesame````, or ````QWxhZGRpbjpvcGVuIHNlc2FtZQ==````. Then the Authorization header field will appear as:

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==

## OWASP auth cheatsheet

**Define the authentication process to a non-technical recruiter.**
- Imagine you want to enter a private room where there are only confidential files that only you can access, you enter that room by your finger print, if someone else tries to enter that room other than you, the door will not be opened, and that is due to the authentication, the finger print lock machine checks if the finger print that has been scanned is exactly the same as the finger print for whom is authorized to enter that room.

**How should your error messaging respond (both HTTP and HTML)? Why?**

- Error messaging in both HTTP responses and HTML pages should be carefully handled to provide meaningful and secure feedback to users. Here are some best practices for error messaging:

- HTTP Responses:
  - Use appropriate HTTP status codes to indicate the nature of the error. For example:
    - 200 OK: Successful response.
    - 400 Bad Request: Invalid request from the client.
    - 401 Unauthorized: Authentication is required.
    - 403 Forbidden: The server understands the request, but the user does not have permission to access the requested resource.
    - 404 Not Found: The requested resource could not be found.
    - 500 Internal Server Error: An unexpected error occurred on the server.

- Include a clear and concise error message in the response body. Avoid revealing sensitive information, such as stack traces or database details, that could aid potential attackers.

- HTML Pages:

  - Present user-friendly error messages that are easy to understand and provide guidance on how to resolve the issue.

  - Avoid disclosing sensitive information in error messages. Instead, provide general information that helps users troubleshoot without compromising security.

  - Consider providing contact information or a support link where users can seek further assistance if needed.
  - Maintain a consistent error message style across the application to enhance usability and familiarity.

- The main reasons for handling error messaging in this way are:

  - Usability: Clear and meaningful error messages help users understand what went wrong and guide them towards resolving the issue. This improves the overall user experience.

  - Security: Revealing detailed error messages with sensitive information can potentially aid attackers in exploiting vulnerabilities or gaining unauthorized access. By providing generalized error messages, the risk of information disclosure is minimized.

  - Compliance: Following best practices for error messaging helps meet security and privacy standards, such as those outlined by OWASP or various industry-specific regulations.

  - It's important to strike a balance between user-friendliness and security when handling error messaging, ensuring that users receive helpful information while minimizing the risk of exposing sensitive data.

**Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle.**

- The statement emphasizes the importance of bookmarking a specific link and considering OWASP (Open Web Application Security Project) fundamentals whenever interacting with authentication. It also highlights that applications developed with security as a core consideration from the beginning tend to have fewer vulnerabilities throughout their lifecycle.

- By bookmarking the provided link, you can access relevant information or resources related to authentication and stay updated on best practices and security measures. The mention of OWASP fundamentals suggests referring to the guidelines and recommendations provided by OWASP, a widely recognized organization that focuses on improving web application security.

- Taking OWASP fundamentals into account when dealing with authentication means incorporating secure coding practices, implementing strong authentication mechanisms, protecting against common vulnerabilities (such as injection attacks, session management flaws, etc.), and following other security measures outlined by OWASP.

- By prioritizing security during the development process, applications can mitigate potential vulnerabilities and reduce the risk of security breaches or unauthorized access, ensuring a more robust and secure overall system.
