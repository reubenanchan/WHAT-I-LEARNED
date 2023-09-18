# Encrypting with Block Ciphers

## Block Ciphers
- Encryption of fixed length chunks of bits (called "blocks")
- Each block is encrypted separately

Keygen
: Accepts a security parameter k, outputs a random k-bit

>$Gen: k \rightarrow (0,1)^k$

Encrypt
: accepts a b-bit plaintext and k-bit key and outputs a b-bit ciphertext

>$Enc: (0,1)^b \times (0,1)^k \rightarrow (0,1)^b$

Decrypt
: Accepts a b-bit cipher and k-bit key amd outputs a b-bit plaintext

>$Dec: (0,1)^b \times (0,1)^k \rightarrow (0,1)^b$

### An Ideal Block Cipher
Encryption is Injective and Surjective.
Injective + Surjective = Bijective. This means every plaintext is associated with a unique ciphertext, and vice versa


Encryption is a permutation (shuffle) of b-bit strings.