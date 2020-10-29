STRIDE
Building a secure software involves taking a few factors into consideration. In securing the  software, we may use the STRIDE framework, which has six areas of focus:
•	Spoofing
•	Tampering
•	Repudiation
•	Information Disclosure
•	Denial of Service
•	Elevation of Privilege

Spoofing

Trust must be established before granting users and services access to your system. Every access must be authenticated. The security of your systems depends upon trust in the other party’s identity. A threat to this trust is spoofing — when someone claims to be a person or system they are not. In these systems, passwords, keys, tokens, and signatures are among the methods used to authenticate requests. The level of vulnerability varies based on the method.

Here are some common authentication methods for systems and what would be required to spoof a request:
•	Single key: many APIs use a single API Key to authenticate requests to their service. The value is static, though it can typically be deleted and regenerated in a user interface. Anyone who obtains the key would have access to the systems that trust it indefinitely.
•	Access token: similar to the single key, an access token is one value that authenticates a request. However, the access is usually limited in some way, often only usable for a short period. Anyone with an access token would only have minimal usage before needing additional credentials to generate another token.
•	Signatures: in contrast to the other two methods, signature-based authentication uses encryption, which requires private keys. Each request is signed using a shared secret that you can verify. To spoof a signature, the attacker would need access to the sender's private key.
To prevent spoofing,  make sure the right mechanism is used to communicate identity and how you know the identity can be trusted.

Tampering

Reliable data is important in our system. Data is especially susceptible to threats of tampering, but physical machines or hardware may also be vulnerable. To prevent tampering with our network systems, we may use Firewalls and partitioned storage among other techniques. We could also use Log files to detect tampered data.

Repudiation

Although attempted security threats can’t be prevented, we can implement auditing to catch and trace attacks. Done correctly, you can be certain that these nefarious efforts can be connected to the source of the vulnerability. Secure systems should build in non-repudiation mechanisms, such that the data source and the data itself can be trusted. For this reason, repudiation is intertwined with other elements of the STRIDE framework. 

Information Disclosure

private information may be accidentally exposed by any system that stores or accesses them. There are any number of methods that can be used to access private data. These disclosures can impact individuals as well as businesses. Data breaches have exposed users’  passwords, payment details, and other expensive personal data. Devices such as servers, laptops, or external drives containing sensitive data should be secured at all times. 




Denial Of Service

Another security threat from the technical is a denial of service makes a system unreachable by exploiting resources so they can’t be used for legitimate purposes. In networking, this can mean overloading a system with incoming requests, making it impossible for users to connect.
You should consider all areas of your system that might be subject to a denial of service threat. 

Elevation Of Privilege

in the STRIDE framework, we’re also concerned about elevation of privilege. In other words, the attacker not only claimed to be a valid user, but one with an expanded role.
A sophisticated elevation of privilege attack may use all of the other areas of STRIDE for an especially outsized impact. With admin access, the attacker may be able to tamper with systems outside of the typical interfaces. The lack of audit trail could cause both repudiation and information disclosure without any trace. 
