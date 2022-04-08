# TLS
* TLS=Transport Layer Security
* [How TLS works](../documents/sg07_encrypting_network.pptx)
* Java programs use keystores. Other programs use the pem files. This is why CDP deploys both keystores and pem files.

## Enable Auto TLS in CM
* [create a jssecacerts.pem file to be used by Auto-TLS](../documents/mod16_ex01__creating_the_jssecacerts_pem_file.pdf)
* [Configure AUto TLS](../documents/mod16_ex02__deploying_auto_tls.pdf)
* [Verify Auto TLS](../documents/mod16_ex03__verify_auto_tls.pdf)

## How to create certificates
* [Create CA](../documents/mod17_ex01__creating_a_ca.pdf)
* [Creating Global Truststore](../documents/mod17_ex02__creating_global_truststore.pdf)
* [Creating Local Keystore](../documents/mod17_ex03__creating_local_keystore.pdf)
   * When a large enterprise embraces TLS one immediate result will be the requirement to manage an increasing number of private keys and public certificates.
   * The Java community create a solution named Java Keystores.
   * As the name implies the solution is intended to store many keys in a single binary file, called a keystore. This reduces the administration of keys and certificates.
   * The keystore is a binary file that holds keys. It is commonly used to hold both private keys and public keys.
   * It will hold keys from a variety of formats, the two most common being pem and pkcs.
 * [Creating Client Keystore](../documents/mod17_ex04__creating_client_keystore.pdf)
 * [Create local truststore](../documents/mod17_ex05__creating_local_truststore.pdf)
 * [Understanding the x509 Standard](../documents/mod17_ex06__managing_x509_format.pdf)
