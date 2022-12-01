# What is Mimikatz?

Mimikatz is an open-source application that allows users to view and save authentication credentials such as Kerberos tickets. Attackers commonly use Mimikatz to steal credentials and escalate privileges because in most cases, endpoint protection software and antivirus systems will not detect or delete the attack.

Mimikatz can perform credential-gathering techniques such as:

Pass-the-hash: Windows used to store password data in an NTLM hash, and Mimikatz can pass that exact hash string to the target computer to log in.

Pass-the-ticket: Newer versions of Windows store password data in a construct called a ticket, and Mimikatz provides functionality for a user to pass a Kerberos ticket to another computer and log in with that user’s ticket.

Overpass-the-hash (pass-the-key): This technique passes a unique key obtained from a domain controller to impersonate a user.

Kerberoast golden tickets: This is a pass-the-ticket attack, but it’s a specific ticket for a hidden account called KRBTGT, which is the account that encrypts all of the other tickets.

Kerberoast silver tickets: Another pass-the-ticket, but a silver ticket takes advantage of a feature in Windows that makes it easy for you to use services on the network. 

Pass-the-cache: A pass-the-cache attack is generally the same as a pass-the-ticket, but this one uses the saved and encrypted login data on a Mac/UNIX/Linux system.

How to defend against Mimikatz:

- Restrict admin privileges. 

- Disable password-caching.

- Turn off debug privileges.

- Configure additional local security authority (LSA) protection.

Reference: https://www.varonis.com/blog/what-is-mimikatz
