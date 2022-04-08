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
   * krdb5kdc daemon
     * Key Distribution Center daem
     * It is responsible for authentication and ticket grants
   * kadmind daemon
     * Kerberos administration daemon
     * It is responsible for the secure database and the management of principals and secret keys

## Kerberos and DNS
* Kerberos does not use IP’s
* Kerberos is highly dependent on DNS and reverse DNS.

## Key Terms for Kerberos

### Realm 
* A domain of hosts using the Kerberos services
   * EXAMPLE.COM
* By convention the Kerberos realm is ALL CAPITALS
### Principals 
* The end-users and services using Kerberos
    * primary/instance@REALM
### Keytab 
* A file holding the name of the principal and the secret key
   * /etc/security/keytabs/nn.service.keytab
### Secret Key 
* An algorithm encrypts the password, which is stored in the Kerberos database and within the keytab, it is used to identify the principal
   * #$(HK#O35HE?@#2367

* hdfs/master01.example.com@EXAMPLE.COM
   * There are called Sevice princiapl 
   * hdfs = Principals
   * master01.example.com = Host address(Optional)
   * EXAMPLE.COM = Realm

* There is a headless principal as well
   * jisahma1@OS.NET.IBM.COM

## Kerberos Tickets
### Ticket Granting Tickets (TGT)
* A ticket granted to an authenticated user 
* Grants rights to request tickets to individual services

### Ticket Granting Services (TGS)
* A ticket granting access to a specified service
* Tickets have a time to live (TTL).

## Kerberos commands
* An admin tool used only on server
```
Kadmin.local
```
* An admin tool for remote access
```
Kadmin
```
* The admin tool for the keytab database
```
kdb5_util
```
* CLI for creating and updating keytab files
```
kutil
```
* CLI for requesting tickets
```
kinit
```
* Listing tickets
```
klist
```
* Releasing tickets
```
kdestroy
```

## Unsecure and secure Access
* Unsecure access to Hive
```
beeline -u "jdbc:hive2://localhost:10000/default”
```
* Secured access to Hive using the default binary transport mode
```
beeline -u "jdbc:hive2://localhost:10000/default;principal=hive/_HIVE@EXAMPLE.COM”
```

## Exercise
* [introducing the Kerberos Command Line Interface (CLI)](../documents/mod18_ex01__using_kerberos_cli.pdf)
* [use Cloudera Manager’s Kerberos wizard to deploy Kerberos](../documents/mod18_ex02__deploying_kerberos.pdf)
* [Verify Kerberos and SASL in CM](../documents/mod18_ex03__verify_kerberos_and_sasl.pdf)
* 









