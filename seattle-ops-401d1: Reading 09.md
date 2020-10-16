Public Key Infrastructure (PKI)

A technology for authenticating users and devices (entities) in the digital world. The idea is to have one or more trusted parties digitally sign documents certifying that a particular cryptographic key belongs to a particular user or device. The key can then be used as an identity for the user in digital networks. The trusted party signing the document associating the key with the device is called a certificate authority (CA). 

The certificate authority uses cryptographic keys known as certificates to sign the documents. 

A public key infrastructure relies on digital signature technology, which uses public key cryptography. The basic idea is that the secret key of each entity is only known by that entity and is used for signing. This key is called the private key.

Common Uses of Certificates

Secure Web Sites - HTTPS
The most familiar use of PKI is in SSL certificates. SSL (Secure Sockets Layer) is the security protocol used on the web when you fetch a page whose address begins with “https” - TLS (Transport Layer Security) is a newer version of the protocol. Certificates and cryptographic authentication of the server prevent man-in-the-middle attacks.

Authenticating Users and Computers - SSH
The Secure Shell protocol supports certificates for authenticating hosts and users. Tectia SSH uses standards-based X.509 certificates, whereas OpenSSH uses its own proprietary certificate formats.

Email Signing and Encryption
Certificates are also used for secure email in corporations. The S/MIME standard specifies a message format for signed and encrypted messaging, using the X.509 certificate formats.
PGP (Pretty Good Privacy) and its free version, Gnu Privacy Guard (GPG), use their own certificate format and a somewhat different trust model. However, they still offer email encryption.

Security Limitations of Public Key Infrastructure
The main weakness of public PKI is that any certificate authority can sign a certificate for any person or computer. Certificate authorities exist in many countries, some of which have rather authoritarian or even potentially hostile governments. Sometimes certificate authorities create or are coerced to create certificates for parties they have no business vouching for.
Intelligence agencies can use fraudulent certificates for espionage, malware injection, and forging messages or evidence to disrupt or discredit adversaries. Some organizations run their own private public key infrastructures. This means they run their own internal certificate authority which helps cost savings.

SSH's Role in the Development of Public Key Infrastructure
SSH Communications Security was one of the early pioneers in PKI, who participated in the standardization work for X.509v3 and proposed an alternative Simple Public Key Infrastructure (SPKI) approach to address some of the trust issues with the X.509 standard.

