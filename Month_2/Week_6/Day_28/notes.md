Day 28: Introduction to Data Encryption
Core Concept:
Data Encryption is the process of converting plaintext (readable data) into ciphertext (scrambled, unreadable data) to ensure confidentiality. It is a fundamental application of the science of Cryptography.

Key Types of Encryption:

Symmetric Encryption:

Definition: Uses a single, shared secret key for both encryption and decryption.

Analogy: Like a physical key that locks and unlocks the same door.

Challenge: Secure key distribution. How do you safely give the secret key to the intended recipient?

Examples: AES (Advanced Encryption Standard), DES (Data Encryption Standard).

Asymmetric Encryption (Public Key Cryptography):

Definition: Uses a mathematically linked key pair: a Public Key (shared openly) and a Private Key (kept secret).

How it works:

Data encrypted with a public key can only be decrypted by its corresponding private key.

This solves the key distribution problem of symmetric encryption.

Examples: RSA, Elliptic Curve Cryptography (ECC).

Critical Application:
Public Key Cryptography is the foundation for many modern security protocols.

SSL/TLS (Secure Sockets Layer / Transport Layer Security): The protocol that enables secure HTTPS connections on the web. It uses asymmetric encryption to establish a secure session and then exchanges a symmetric key for faster bulk data encryption.