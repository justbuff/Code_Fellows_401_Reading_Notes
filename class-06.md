# Data File Encryption

## Applying The CIA Triad To Your Enterprise File Transfer

The CIA Triad refers to three basic principles/objectives in information security: confidentiality, integrity, and availability.

- Confidentiality: In the context of information security, confidentiality refers to the principle of restricting access to or knowledge of certain pieces of information to certain individuals.

- Integrity: The second member of the CIA triad, integrity (which means data integrity) pertains to the principle of preventing data from being tampered. 

Note: Confidentiality and integrity can be compromised during data transfers through either man-in-the-middle attacks (where attackers can intercept the data, make changes, and then forward the altered data to the intended recipient) or through a direct hack on the server.

- Availability: the process of ensuring that data is available to end-users and applications, when and where they need it.

Encryption basically renders data unreadable, preserving that data's confidentiality. The data can become readable again only after it's decrypted.

Encryption solutions are usually grouped into two categories: 

- Data-at-rest: usually achieved through OpenPGP or other disk-level or file-level encryption solutions.
 
- Data-in-transit: usually achieved through solutions like SSL (e.g. FTPS, HTTPS, WebDAVs) or SSH (e.g. SFTP).

Another method you can use to secure data confidentiality is authentication, whichcan help you restrict access to your confidential data to authorized individuals, such as implementing 2-factor authentication.

To achieve data integrity in your file transfers, you can use hash functions and digital signatures, security elements that are readily available in secure file transfer protocols like FTPS, HTTPS, SFTP, and WebDAVs.

## What Are MD5, SHA-1, and SHA-256 Hashes, and How Do I Check Them?

Hashes are the products of cryptographic algorithms designed to produce a string of characters. Often these strings have a fixed length, regardless of the size of the input data. MD5, SHA-1, and SHA-256 are all different hash functions.

Note: "Collisions” have been found with the MD5 and SHA-1 functions, which are multiple different files that result in the same MD5 or SHA-1 hash. That’s why you should prefer SHA-256 when possible.

While hashes can help you confirm a file wasn’t tampered with, there’s still one avenue of attack here. An attacker could gain control of a Linux distribution’s website and modify the hashes that appear on it, or an attacker could perform a man-in-the-middle attack and modify the web page in transit if you were accessing the website via HTTP instead of encrypted HTTPS.
