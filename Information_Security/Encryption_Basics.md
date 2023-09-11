# Encryption Basics

# Terminology

**Plaintext**
: Unencrypted information. What you want to encrypt.

**Ciphertext**
: Encrypted plain text. Looks totally random.

**Key**
: Secret to transform between plaintext and ciphertext

**Plaintext Space**
: Set of valid plaintexts

**Ciphertext Space**
: Set of valid ciphertexts

**Key Space**
: Set of valid keys

## Encryption Functions

Encryption contains three functions

1. **Key Generation Function:** The process of generating keys for cryptography
    ![Alt text](<../Images/Infomation Security/keygen.png>)
2. **Encryption function:** takes the key and converts the plaintext into ciphertext.
    ![Alt text](<../Images/Infomation Security/encryption function.png>)
3. **Decryption function:** takes the key and converts the ciphertext into plaintext.
    ![Alt text](<../Images/Infomation Security/decyption function.png>)

## Properties of Good Encryption

1. **Efficient:** Encryption, decryption, and key generation are efficiently computable.
2. **Unique Decryption:** Decrypting the encryption of a message always returns the original message.
3. **Confidential:** Difficult to extract information about the plaintext without the key.
4. **Secure:** It should be hard to guess the key, even with knowledge of plaintext/cipthertext pair.

## Classical Ciphers[^1]

Substitution Ciphers
: Swapping one letter for another

### Ceasar Cipher

 A substitution cipher that shifts letters in a message to make it unreadable if intercepted.

 The Key is the amount shifts.

 ![Alt text](<../Images/Infomation Security/ceasar.png>)

 >The Problem with this cipher is that it can be easily hacked. By looking at the pattern of the letters in it, the entire message can be decrypted.

### Vigenere Cipher

 A method of encrypting alphabetic text where each letter of the plaintext is encoded with a different Caesar cipher, whose increment is determined by the corresponding letter of another text, the key.

![Alt text](<../Images/Infomation Security/vigenere.png>)

### Enigma Cipher
The Enigma has an electromechanical rotor mechanism that scrambles the 26 letters of the alphabet.

![Alt text](<../Images/Infomation Security/enigma.png>)

[^1]: Use slides as reference