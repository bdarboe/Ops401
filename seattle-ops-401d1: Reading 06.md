                                                                    Data file encryption

                                                                        CIA Triad
                                                                        
CIA Triad which stands for Confidentiality, Integrity, and Availability is very important in establishing secure enterprise file transfer. 
Confidentiality in business file transfer refers to the secure transfer of information from one party to the other without the information falling in the hands of an unauthorized party. Confidential information may be acquired when attackers establish a man in the middle approach to acquire secure information. In confidentiality, encryption is highly utilized to make the data unreadable by unintended audience. Authentication is a method that is also utilized to verify the user before permissions are granted – for example using the well two factor authentication.

In integrity, refers to the protection of data and preventing it from being compromised. Caution has to be put in place to prevent data from falling in the wrong hands. The integrity of your data can be achieved by using different types of technologies such as hash functions and digital signatures. We can use file transfer protocols such FTPS, HTTPS, SFTP, and WebDAV. The receiver can then determine if the file has be altered on its route.

Availability makes sure that you can preserve the confidentiality and integrity of your data at all times. However, your data may be subject to attacks and failures therefore rendering your data inaccessible. Availability can have serious problems especially with the involving of other organizations and businesses.  Availability should be set up as high and one or two failovers in case the primary server malfunctions or fail. Two servers can also be setup to run side-by-side in order to distribute the load and avoiding one server carrying all the load. 

The implementation of all three elements can be complicated, so a single solution with all three elements could be a better solution. For example JSCAPE MFT Server, which includes: 
•	Data-in-motion encryption through secure file transfer protocols like FTPS, SFTP, HTTPS, WebDAVs, AS2 over HTTPS, and OFTP (secured by SSL)
•	Data-at-rest encryption through OpenPGP 
•	End-to-end encryption, which can be achieved through automation-enabling features known as triggers. 
•	2-factor authentication
•	Data integrity checking mechanisms that employ hash functions and digital signatures.
•	Built-in support for High Availability configurations, active-active and active-passive
•	Data Loss Prevention (DLP), which automatically detects the presence of sensitive data and take appropriate action (e.g. cancel the download or apply encryption)

                                                                           Hashes
                                                                           
Hashes are cryptographic algorithms that produces strings of characters usually with a fixed size output irrespective of the size of the input. Hashes changes each time a data is modified even a minute modification can produce a significant hash change. Hash functions are used in verifying that a file has not been altered by checking the original hash and match it to your own hash. However, attackers may hack the system that host the original file and modify the original. In case of the modification of the original file, users risk running a tampered file. Linux distribution have made it so that users can verify the signature as well. 

In Windows, the following powershell command is run to get the hash for your file:
Get-FileHash C:\path\to\file.iso

In MacOS, we run the following commands for MD5, SHA-1, and SHA-256 hashes:
md5 /path/to/file
shasum /path/to/file
shasum -a 1 /path/to/file
shasum -a 256 /path/to/fi

In Linux we run the following commands.
md5sum /path/to/file
sha1sum /path/to/file
sha256sum /path/to/file

MD5, SHA-1, and SHA-256 are different hash functions, SHA-256 has been known to be the most reliable and recommended.
