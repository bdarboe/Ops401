					What is cross-site scripting (XSS)?

Cross-site scripting (also known as XSS) is a web security vulnerability that allows an attacker to compromise the interactions that users have with a vulnerable application by masquerading as a user. The attacker by-pass the same origin policy, which is designed to segregate different websites from each other. XSS works by manipulating a vulnerable web site so that it returns malicious JavaScript to users, enabling the attacker to fully compromise their interaction with the victim's application.

					What are the types of XSS attacks?

Reflected XSS, where the malicious script comes from the current HTTP request.
Stored XSS, where the malicious script comes from the website's database.
DOM-based XSS, where the vulnerability exists in client-side code rather than server-side code.

					What can XSS be used for?

An attacker who exploits a cross-site scripting vulnerability is typically able to:

Impersonate or masquerade as the victim user.

Carry out any action that the user is able to perform.

Read any data that the user is able to access.

Capture the user's login credentials.

Perform virtual defacement of the web site.

Inject trojan functionality into the web site.

					 Impact of XSS vulnerabilities

In a brochureware application, where all users are anonymous and all information is public, the impact will often be minimal.

In an application holding sensitive data, such as banking transactions, emails, or healthcare records, the impact will usually be serious.

If the compromised user has elevated privileges within the application, then the impact will generally be critical, allowing the attacker to take full control of the vulnerable application and compromise all users and their data.

					How to find and test for XSS vulnerabilities

The vast majority of XSS vulnerabilities can be found quickly and reliably using Burp Suite's web vulnerability scanner.

Manually testing for reflected and stored XSS normally involves submitting some simple unique input (such as a short alphanumeric string) into every entry point in the application; identifying every location where the submitted input is returned in HTTP responses; and testing each location individually to determine whether suitably crafted input can be used to execute arbitrary JavaScript.

					Content security policy

Content security policy (CSP) is a browser mechanism that aims to mitigate the impact of cross-site scripting and some other vulnerabilities. 

					How to Prevent XSS attack

In general, effectively preventing XSS vulnerabilities is likely to involve a combination of the following measures:

Filter input on arrival. 

Encode data on output. 

Use appropriate response headers. 

Content Security Policy. 
