[![Build Status](https://travis-ci.org/EC-SEAL/derivation-id.svg?branch=development)](https://travis-ci.org/EC-SEAL/derivation-id)

# Derivation-id
Seal derivation ID Module

The following steps need to be made in order to run the derivation ID microservice

#### 1. Environmental variables

The following environmental variables need to be set prior to running the project:

|Environment       | Description |
|------------------| ---- | 
| ASYNC_SYGNATURE  | Boolean value, if true denotes RSA signing for JWTs, else HS256 signing is conducted.|
| KEY_PASS         | Password for the certificate| 
| STORE_PASS       | Password for the keystore containing the certificate.| 
| HTTPSIG_CERT_ALIAS | Alias of the certificate used for the httpSig protocol. |
| SESSION_MANAGER_URL| Location of the Session Manager microservice. |
| CONFIGURATION_MANAGER_URL| Location of the Config Manager microservice. |
| KEY_STORE_PATH   |Path to the keystore holding the RSA certificate used for signing JWTs. 
| SAML_KEYSTORE_PATH |
| SAML_KEYSTORE_PASS |
| SAML_KEYSTORE_ID |
| SAML_KEY_PASS |
| EXPIRATION_WINDOW | Expiration time in "day of the year" that the linkService is expected to be received.



#### 2. Run


After setting the environmental variables, just run: 

```mvn spring-bot:run ```


#### 2. Test
Runs unit tests 


```mvn spring-bot:test ```

