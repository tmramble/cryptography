

### Project Title: Cryptography Lab Report: Exploring Encryption Techniques and Data Security

#### Summary:
This report documents my work in the COP 610 Cryptography Lab, where I explored various encryption techniques, symmetric key algorithms, and their implications for data security. Through hands-on experiments using tools such as OpenSSL and Wireshark, I gained insights into symmetric key encryption, Public Key Infrastructure (PKI), and the vulnerabilities associated with hash functions.

Key Accomplishments
- Conducted symmetric key encryption using various ciphers and modes.
Deployed certificates for an HTTPS web server using OpenSSL.
Configured an Apache server to support self-signed certificates.
Analyzed the effects of changing encryption parameters like key and IV values.
Utilized Wireshark to demonstrate data visibility in HTTP and HTTPS.
Performed frequency analysis to decrypt messages and discover encryption keys.
Resolved challenges encountered during certificate generation and server configuration.


#### Project Details:

**1. Lab 1 – Symmetric Key Lab**

- **Monoalphabetic Substitution Cipher:**
  - I decrypted a secret message using a monoalphabetic substitution cipher. The encryption key discovered was: *‘fpdyehjbgiknvrmlusxwotczaq’*.
  
- **Encryption Using Different Ciphers and Modes:**
  - I used OpenSSL commands to encrypt and decrypt files using different cipher modes, including AES-128-CBC. Specific commands included:
    - For encryption: `openssl enc -aes-128-cbc -e -in myfile.txt -out mycipher.bin -K 0011223344556677889aabbccddeeff -iv 0102030405060708`
    - For decryption: `openssl enc -aes-128-cbc -d -in mycipher.bin -out myd.txt -K 0011223344556677889aabbccddeeff -iv 0102030405060708`
  - I experimented with changing the initialization vector (IV) and observed that using the same IV with different plaintexts resulted in identical ciphertexts, highlighting the importance of unique IVs for security.

- **Initial Vector (IV):**
  - I listed OpenSSL commands used to demonstrate the impact of IV on encryption. I learned that a unique IV is crucial as reusing an IV can lead to vulnerabilities in encrypted data.

**2. MARS – Data Visibility with Wireshark**

- **Form Data Visibility:**
  - I utilized Wireshark to capture data packets from HTTP and HTTPS form submissions. Specific Wireshark filters helped me analyze packet data visibility.
  - I demonstrated how form data is visible in HTTP requests but encrypted and secure in HTTPS.

- **Packet Capture Experimentation:**
  - I initiated a packet capture session using Wireshark and analyzed the saved capture file. This exercise emphasized the utility of packet capture for understanding network traffic and troubleshooting.

**3. Lab 2 – PKI Lab**

- **Deploying Certificate in an HTTPS Web Server:**
  - I faced challenges while generating certificates and configuring OpenSSL for testing. I successfully resolved these by following documentation and troubleshooting common issues.

- **Deploying Certificates in an Apache-Based HTTPS Website:**
  - I successfully configured an Apache server to use self-signed certificates. I gained practical experience in web server security and SSL/TLS configurations.

**4. Hash Length Extension Attack:**
  - I reviewed the implications of insecure MAC computation and the vulnerabilities associated with hash functions. I explored HMAC as a mitigation strategy, understanding that it provides stronger security against length extension attacks.

#### Tools Used:
- **OpenSSL:** For encrypting and decrypting files using various ciphers and modes.
- **Wireshark:** To analyze network traffic and assess data visibility in HTTP and HTTPS protocols.
- **Linux Terminal:** For executing commands, creating files, and managing encryption tasks.

#### Conclusion:
Through this lab project, I deepened my understanding of cryptographic techniques, their implementation using industry-standard tools, and the critical importance of secure practices in data handling. The hands-on experience has equipped me with practical skills that are essential for a career in cybersecurity and cryptography.

--- 

