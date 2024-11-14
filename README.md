# INSE6110 Project - Exploring and Enhancing Security Protocols in Network Communications

## Project Title
**Implementing Authentication and Encryption Mechanisms in Network Communications**

This repository contains my individual project work for **INSE6110, Fall 2023**, focusing on implementing authentication and encryption techniques to enhance security protocols in network communications. The goal of this project was to develop a secure workflow for message encryption, decryption, and digital signature verification.

---

## Project Overview

This project demonstrates essential cryptographic practices, including public key generation, message encryption and decryption, and digital signatures. These components are critical for ensuring data confidentiality, integrity, and authenticity in secure communications.

---

## Objectives

1. **Develop** a public and private key generation system for secure communications.
2. **Implement** encryption and decryption functions to protect message confidentiality.
3. **Introduce** digital signatures to verify message integrity and authenticity.
4. **Validate** the cryptographic mechanisms with end-to-end testing.

---

## Project Components

The project is organized into five primary Python scripts:

1. **Generating_public_key.py**: Generates a public and private key pair for encryption, decryption, and signing.
2. **Message_Encryption.py**: Encrypts a plaintext message using the public key.
3. **Message_Decryption.py**: Decrypts an encrypted message using the private key.
4. **Signature.py**: Signs a message with the private key to provide a digital signature.
5. **Signature_Verification.py**: Verifies the authenticity of a message by validating its signature with the public key.

Each component plays a role in securing message transmission and ensuring message integrity in a communication setup.

---

## Methodology

To implement and test the authentication mechanisms, I followed these steps:

1. **Key Generation**: Created public and private keys to serve as the foundation for encryption, decryption, and digital signing.
2. **Message Encryption**: Used public-key encryption to secure messages, preventing unauthorized access.
3. **Message Decryption**: Applied private-key decryption to retrieve the original message, demonstrating data confidentiality.
4. **Digital Signature Creation**: Implemented digital signatures to validate sender authenticity.
5. **Signature Verification**: Tested signature validation to ensure message integrity and prevent tampering.

Each step was verified by simulating communication scenarios and ensuring that the cryptographic functions behaved as expected.

---

## How to Run

### Prerequisites

- **Python 3.x**
- **Cryptography Library**: Install via `pip install cryptography`

### Instructions

1. **Generate Keys**:
   ```bash
   python Generating_public_key.py
   ```
   This will create `public_key.pem` and `private_key.pem` files for further encryption and signing.

2. **Encrypt a Message**:
   ```bash
   python Message_Encryption.py
   ```
   Enter a message when prompted. The encrypted message is saved as `encrypted_message.txt`.

3. **Decrypt the Message**:
   ```bash
   python Message_Decryption.py
   ```
   Decrypts `encrypted_message.txt` using the private key, displaying the original message.

4. **Sign a Message**:
   ```bash
   python Signature.py
   ```
   Enter a message when prompted. The generated signature is saved as `signature.sig`.

5. **Verify a Signature**:
   ```bash
   python Signature_Verification.py
   ```
   Verifies `signature.sig` against the provided message using the public key, confirming message integrity.

---

## Project File Structure

```plaintext
CryptoProject
├── Generating_public_key.py         # Generates public and private keys
├── Message_Encryption.py            # Encrypts a message
├── Message_Decryption.py            # Decrypts a message
├── Signature.py                     # Signs a message
├── Signature_Verification.py        # Verifies a message signature
├── public_key.pem                   # Public key file (generated)
├── private_key.pem                  # Private key file (generated)
├── encrypted_message.txt            # Encrypted message (generated)
└── signature.sig                    # Digital signature (generated)
```

---

## Acknowledgments

This project was completed as part of **INSE6110** coursework at Concordia University, **Fall 2023**. I would like to thank **Ayda Basyouni** for his guidance in understanding and applying cryptographic concepts.

--- 

This README includes a structured description of your cryptographic project, detailing each script’s function and providing clear instructions for usage. Let me know if you'd like further customization!
