# Security Goals and Principles

## Cybersecurity

The practice of protecting computers, servers, mobile devices, networks and data from unauthorized, disclosure access and modification.

### Types of Cybersecurity

1. **Information Security:** Protecting information with cryptography and secure communication protocols.
[^1]
2. **Software Security:** Preventing the exploitation of vulnerabilities and execution of malicious code
3. **Systems Security** Preventing unauthorized/unprivileged access to cyber to access to cybersecurity and resources

## Security Principles

- **Confidentiality:** Keep information from non authorized parties.
- **Integrity:** Detect information sent by an authorized party.
- **Availability:** Access for authorized parties to access an information system
- **Authenticity:** Ability of an authorized party to prove its identity to another

## Mental Model of Communication Security

![Alt text](<../Images/Infomation Security/communication model.png>)

**Eavesdropper**
: an attacker intercepts and listens to communications between two parties without their knowledge or consent

![Alt text](<../Images/Infomation Security/eavesdropping.png>)

**Man-In-The-Middle (MITM)**
: A man in the middle (MITM) attack is a general term for when a perpetrator positions himself in a conversation between a user and an application—either to eavesdrop or to impersonate one of the parties, making it appear as if a normal exchange of information is underway.

![Alt text](<../Images/Infomation Security/MITM.png>)

## Kerkhoff's Principle

The concept in which Cryptographic systems should designed to be secure, even if all its details, except for the key, are publicly know.

>Security by **design**, not security though **obscurity**

## Brute Force & Bits of Security

**Brute Force**
: a cryptographic hack that relies on guessing possible combinations of a targeted password until the correct password is discovered.

### Bits of Security

log_2 (Number of combinations you expect to have to try)

How many bits of security is reasonable?
> Approximately 120 bits. To crack 128-bit encryption using a brute force attack, the answer would be 1 billion years


[^1]: course only on this section.





