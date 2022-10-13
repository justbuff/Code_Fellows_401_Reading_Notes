# Public Key infrasctructure (PKI)

PKI is a technology for digitally authenticating users and devices. One or more trusted parties digitally sign documents certifying that a particular cryptographic key belongs to a particular user or device. The key can then be used as an identity for the user in digital networks. The users and devices that have keys are often called entities. The purpose of a PKI is to securely associate a key with an entity.

The secret key of each entity is only known by that entity and is used for signing, and is known as the private key. There is another key derived from it, called the public key, which is used for verifying signatures but cannot be used to sign. This public key is made available to anyone, and is typically included in the certificate document.

The trusted party signing the document associating the key with the device is called a certificate authority (CA). The certificate authority also has a cryptographic key that it uses for signing these documents. These documents are called certificates.

Most public key infrastructures use a standardized machine-readable certificate format for the certificate documents. The standard is called X.509v3. 

The main weakness of public PKI is that any certificate authority can sign a certificate for any person or computer.

Common Uses of Certificates:

- Secure Web Sites - HTTPS

- Authenticating Users and Computers - SSH

- Email Signing and Encryption
