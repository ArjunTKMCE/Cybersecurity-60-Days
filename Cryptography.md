# Cryptography Basics

## Symmetric Cryptography
Uses one shared secret key for encryption and decryption. It is efficient for large amounts of data.

## Asymmetric Cryptography
Uses a public/private key pair. Common uses include digital signatures, key exchange, and certificates.

## Hashing
A hash produces a fixed-size digest.

```bash
md5sum test.txt
sha256sum test.txt
```

MD5 is cryptographically broken and should not be used for modern security purposes. SHA-256 is commonly used when an SHA-2 hash is appropriate.

## Digital Certificates
Certificates bind an identity/domain to a public key and are commonly issued by Certificate Authorities in real-world PKI.

## TLS
TLS provides encryption and authentication for protected network communication such as HTTPS.

## OpenSSL Practical
```bash
openssl version
openssl genrsa -out private.key 2048
openssl rsa -in private.key -pubout -out public.key
openssl req -x509 -new -key private.key -out certificate.crt -days 365
openssl x509 -in certificate.crt -text -noout
```
