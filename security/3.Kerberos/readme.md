# Kerberos
* Is used for authentication.
* A project driven by MIT
* Kerberos provides trusted and proven security management for large clusters.

## Key Attributes of Kerberos
* Provides strong authentication
* Establishes identity for users, services and host
* Prevents impersonation on unauthorized account
* Supports token delegation model
* Works with existing directory services
* Highly scalable, as principals and services only need to know their own secret keys
* Light weight, only runs two daemons on the server.

## Kerberos and DNS
* Kerberos does not use IP’s
* Kerberos is highly dependent on DNS and reverse DNS.

## Key Terms for Kerberos

### Realm 
* A domain of hosts using the Kerberos services
   * EXAMPLE.COM
### Principals 
* The end-users and services using Kerberos
    * primary/instance@REALM
### Keytab 
* A file holding the name of the principal and the secret key
   * /etc/security/keytabs/nn.service.keytab
### Secret Key 
* An algorithm encrypts the password, which is stored in the Kerberos database and within the keytab, it is used to identify the principal
   $ #$(HK#O35HE?@#2367



