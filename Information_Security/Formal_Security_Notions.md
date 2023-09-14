# Formal Security Notions

## The One-Time Pad

- Similar to Vigenere
- Key is exactly the **same length** as the message
- Key is **uniformly random.** Every key in the keyspace is equally likely to be chosen.
- Key is **never** reused.
![Alt text](<Images/Infomation Security/one-time.png>)

## Information-Theoretic Security
A cryptosystem is considered to have information-theoretic security is the system is secure against adversaries with unlimited computing resources and time. In order to achieve this:
- **SOMEHOW** securely transmit one byte of key for EVERY byte of plaintext you want to send
- **SOMEHOW** securely store one byte of key for EVERY byte of plaintext you want to receive
- **SOMEHOW** enforce you never ever reuse a single key byte EVER

## Semantic Security
An encryption scheme is semantically secure, if an adversary cannot guess with better probability than 1/2 whether the given ciphertext is an encryption of message m0 or m1

### Advantage
Advantage is how far off 50% the success rate is.

>$Adv = | Pr(guessing correctly) - \frac{1}{2} |$

Can the advantage ever be 0
> No. since you get the cipthertext, you can try to brute-force decrypt it, and will succeed with some non-zero probability.

### Negligible Function
$\varepsilon$($\lambda$) is a negligible function in security parameter $\lambda$
if for every polynomial function poly(), there is some $\lambda$' > $\lambda$ such that:
>$\varepsilon(\lambda) \le |\frac{1}{poly(\lambda)}|$

In other words, a negligible function shrinks faster than the inverse of any polynomial function.

We have a negligible advantage when:
>$ Adv \le \varepsilon(\lambda)$

## Indistinguishability of Encryption
### IND-EAV Security
A cipher is indistinguishable under eavesdropping (IND-EAV secure)
if there exists no probabilistic polynomial-time Turing machine that
can win the EAV game with a non-negligible advantage

### IND-CPA Security
The **chosen-plaintext attack (CPA)** game runs exactly the same
as the eavesdropping game except the guesser gets an
additional “power:” the ability to make <ins>encryption queries</ins> under
the same key used to create the challenge ciphertext

### IND-CCA1 Security
The **chosen-ciphertext attack (CCA1)** game runs exactly the
same as the CPA game except the guesser gets an additional
“power:” the ability to make <ins>decryption queries</ins> under the same
key as the challenge ciphertext, until the challenge ciphertext is
received

### IND-CCA2 Security
The adaptive **chosen-ciphertext attack (CCA2)** game runs
exactly the same as the CCA1 game except the guesser gets an
additional “power:” the ability to make <ins>decryption queries</ins> after
the challenge ciphertext is received*