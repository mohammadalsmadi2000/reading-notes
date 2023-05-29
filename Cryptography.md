# Cryptography

## Topic Importance:
Cryptography is a crucial topic in the field of computer science and information security. It plays a vital role in ensuring the confidentiality, integrity, and authenticity of sensitive data. Understanding cryptography is essential for anyone studying or working in the field of cybersecurity, as it forms the foundation of secure communication and data protection.

## Reading Questions:

1. What is the basic principle behind the Caesar Cipher, and how was it used historically?
   - The Caesar Cipher is a simple substitution cipher where each letter in the plaintext is shifted a certain number of positions down or up the alphabet. The basic principle behind the Caesar Cipher is the concept of shifting letters to create a secret message. Historically, it was used by Julius Caesar to send secret messages during military campaigns. The shift value, known as the key, determines the amount of shifting applied to each letter.

2. What are the key differences between symmetric and asymmetric encryption? How is asymmetric used in secure communication today?
   - Symmetric encryption uses the same key for both encryption and decryption. The sender and the receiver share the secret key in advance. In contrast, asymmetric encryption, also known as public-key encryption, uses two different keys: a public key for encryption and a private key for decryption. The public key can be freely shared, while the private key remains secret.

   - Asymmetric encryption is widely used in secure communication today. It enables secure key exchange, digital signatures, and secure transmission of sensitive information. For example, when you access a website using HTTPS, asymmetric encryption is used during the initial handshake to securely exchange symmetric session keys, which are then used for the remainder of the communication using faster symmetric encryption.

3. How do computers generate random numbers, and what are the differences between true random number generation (TRNG) and pseudo-random number generation (PRNG)? Discuss their use cases in cryptography.
   - Computers generate random numbers using algorithms called random number generators (RNGs). There are two types of RNGs: true random number generators (TRNGs) and pseudo-random number generators (PRNGs).

   - TRNGs generate numbers based on physical processes that are inherently unpredictable, such as atmospheric noise or radioactive decay. They provide "true" randomness and are suitable for cryptographic purposes where high-quality randomness is required.

   - PRNGs, on the other hand, are algorithms that generate sequences of numbers that appear random but are actually determined by an initial seed value. They are deterministic and repeatable, given the same seed. PRNGs are commonly used in various applications where statistical randomness is sufficient but not necessarily cryptographic security.

   - In cryptography, TRNGs are typically used for generating cryptographic keys, initialization vectors, and other critical random values. PRNGs may be used for non-cryptographic purposes, such as generating random challenges or simulation purposes, but they are not suitable for generating cryptographic keys or ensuring strong security.

4. What's the difference between encryption and decryption? Explain with an analogy.
   - Encryption is the process of converting plaintext into ciphertext using an encryption algorithm and a secret key. It scrambles the original data to make it unreadable to unauthorized parties. An analogy for encryption could be a locked safe. You put your valuables (plaintext) inside the safe, lock it with a key (encryption), and now only someone with the key can unlock it and access the valuables.

   - Decryption is the reverse process of encryption. It involves converting ciphertext back into plaintext using a decryption algorithm and the corresponding secret key. It transforms the scrambled data back to its original form. Analogously, decryption is like unlocking the safe with the correct key to retrieve the valuables stored inside.

## Things I want to know more about

- Advanced encryption algorithms and their applications
- Cryptographic protocols used in secure communication
- Quantum cryptography and its impact on traditional cryptography
