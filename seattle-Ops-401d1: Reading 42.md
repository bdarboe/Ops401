					What is Mimikatz?

An open-source application, developed by Benjamin Delby, that allows users to view and save authentication credentials like Kerberos tickets. Attackers use Mimikatz to steal credentials and escalate privileges and pentesters use it to detect and exploit vulnerabilities in your networks so you can fix them.

					What Can Mimikatz Do?

Mimikatz originally demonstrated how to exploit a single vulnerability in the Windows authentication system. Now the tool demonstrates several different kinds of vulnerabilities. Mimikatz can perform credential-gathering techniques such as:

Pass-the-Hash: Windows used to store password data in an NTLM hash. Attackers use Mimikatz to pass that exact hash string to the target computer to login without cracking the password

Pass-the-Ticket: Mimikatz provides functionality for a user to pass a kerberos ticket to another computer and login with that user’s ticket just like pass-the-hash.

Over-Pass the Hash (Pass the Key): Ppasses a unique key to impersonate a user you can obtain from a domain controller.

Kerberos Golden Ticket: A specific ticket for a hidden account called KRBTGT, which is the account that encrypts all of the other tickets.

Kerberos Silver Ticket: A silver ticket takes advantage of a feature in Windows that makes it easy for you to use services on the network. user is granted a TGS ticket, and a user can use that ticket to log into any services on the network. 

Pass-the-Cache: A pass-the-cache attack is generally the same as a pass-the-ticket, but uses the saved and encrypted login data on a Mac/UNIX/Linux system.
