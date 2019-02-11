# Basic_Terms_To_Know
#### Data at Rest
  * Inactive data that is being stored physically somewhere (e.g. databases, data warehouses, spreadsheets, archives, tapes, off-sites backups, mobile devices)
#### Data in Transit
  * Data in Transit, is data actively moving from one location to another such as across the internet or a Local area Network(LAN)
#### Encryption 
  * The process of converting ordinary information (called plaintext) into unintelligible text (ciphertext).
  * Decryption -> reverse of encryption 
#### Symmetric Encryption
  * Same key is used to encrypt and decrypt
#### Asymmetric Encrytion
  * Different keys are used to Encrypt and Decrypt
#### CipherText 
  * In cryptography, ciphertext or cyphertext is the result of encryption performed on plaintext using an algorithm, called a cipher.
#### HSM (Hardware Security Module)
  * A hardware security module(HSM) is a physical computing device that safeguards and manages digital keys for strong authentication and provides cypto-processing.
#### Customer Managed Key
  * The primary resources in AWS KMS are customer master key (CMKs). You can use CMK to encrypt and decrypt up to 4 KB of data. 
#### Data Keys
  * Keys generated under CMK in KMS that can be used to encrypt large amount of data.
#### Envelope Encryption
  * Envelope encryption is the practice of encrypting plaintext data with a unique data key, and then encrypting the data key with another key.
#### Client-side encryption 
  * is the cryptographic  technique of encrypting data on the sender's side, before it is transmitted to a server such as a cloud storage service. 
#### Server-side encryption
  * is about data encryption at rest - an AWS service encrypts your data as it writes it to disks in its data centers and decrypts it for you when you access it. 
# KMS
#### AWS KMS
  * AWS key managed service is a managed service that makes it easy for you to create and manage encryption keys.
#### 2 types of AWS KMS
  * Customer Managed Keys
  * Data Keys
#### KMS uses Hardware Security Modules (HSMs) to protect the security of your keys. 
#### CMK
  * You can use a CMK to encrypt and decrypt up to 4 KB(4096 bytes)of data.
  * CMK is a logical representation of a master key in AWS KMS.
  * CMK contains the key material used to encrypt and decrypt data. 
  * When you create a CMK, by default AWS KMS generates the key material for the CMK.
  * CMKs can never leave AWS KMS unencrypted. 
  * You create, manage, and use -- CMK.
  * You can allow an AWS service (for eg. AWS S3 or EBS) to use a customer managed CMK on your behalf, but you retain control of the CMK. 
  * AWS managed CMKs have aliases have the format aWS/service-name, such as aws/s3.
  * Typically, a service creates its AWS managed CMK in your account when you set up the service or the first time you use the CMK.
#### 2 Types of CMK
  * Customer Managed
    * KMS generated Key Material 
    * Imported Key Material 
  * AWS Managed
#### Note:
  * You can use your AWS KMS CMKs to generate, encrypt, and decrypt data keys, but AWS KMS doesnot store, manage or track your data keys.
  * AWS KMS cannot use a data key to encrypt data for you. You must use and manage data keys inside your application. 

