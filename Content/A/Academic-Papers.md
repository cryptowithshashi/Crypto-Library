# Academic Cryptography Papers - Annotated

## Overview
This annotated bibliography curates seminal and modern academic papers across cryptography topics including hashing, symmetric cryptography, cryptanalysis, public-key systems, elliptic curves, zero-knowledge proofs, and post-quantum cryptography. Each entry provides concise summaries, significance assessments, and crucially, reproducibility notes highlighting available code, datasets, and replication difficulty. The collection serves researchers, advanced students, implementers auditing cryptographic systems, and reproducibility-minded reviewers seeking both foundational knowledge and practical implementation guidance.

## Why it matters

Literature triage: Cuts through thousands of crypto papers to highlight truly impactful work worth reading first
Implementation guidance: Links to working code, test vectors, and reference implementations for practical deployment
Historical context + modern advances: Bridges foundational theory with current state-of-the-art systems
Reproducibility focus: Emphasizes papers with available artifacts, enabling verification and extension of results
Cross-topic coverage: Spans theoretical foundations to applied systems, supporting diverse research needs

## Scope & inclusion rules

Include seminal/landmark papers (Shannon, Diffie-Hellman, RSA) and high-impact modern results across listed topics
Prefer papers with public code/data or clear experimental protocols; explicitly mark papers lacking artifacts
Include surveys, RFCs, and standards (FIPS documents) where they provide canonical reference implementations
Limit to 30 high-quality entries grouped by topic for focused curation
Mark paywalled items with `paywalled` to aid accessibility assessment
Prioritize papers that balance theoretical contributions with practical implementability


## How entries are annotated
Each entry follows a standardized format: 

- bibliographic information (Title — Authors — Year — Venue), DOI/URL,
- TL;DR (≤50 words summarizing core contribution)
- Significance (≤40 words explaining impact)
- Reproducibility notes (Code availability, Data availability, Replication difficulty rating)
- Notes (up to 2 bullets covering implementation details, hardware requirements, or caveats)
- Tags (2–5 descriptive keywords).


This format enables rapid assessment of both theoretical importance and practical reproducibility.



# Annotated papers 

## Foundations & Information Theory

### 1. A Mathematical Theory of Communication — Claude Shannon — 1948 — Bell System Technical Journal

- DOI: 10.1002/j.1538-7305.1948.tb01338.x
- TL;DR: Establishes information theory foundations including entropy, laying groundwork for cryptographic hash functions and perfect secrecy.
- Significance: Fundamental theoretical basis for all modern cryptography and secure communication systems.
- Reproducibility notes: Code: none found
    - Data: none found
    - Replication difficulty: Easy (mathematical proofs)
  
Notes:
- Purely mathematical work, no computational experiments required
- Essential reading for understanding cryptographic security definitions
- Tags: information-theory, foundations, entropy, classic


### 2. Communication Theory of Secrecy Systems — Claude Shannon — 1949 — Bell System Technical Journal

- URL: http://web.archive.org/web/20201112040412/http://netlab.cs.ucla.edu/wiki/files/shannon1949.pdf
- TL;DR: Establishes theoretical foundations of cryptography including perfect secrecy and unicity distance concepts.
- Significance: Provides mathematical framework for analyzing cryptographic systems and their fundamental limits.
- Data: none found
- Replication difficulty: Easy
  
Notes:

- Introduces one-time pad and proves its perfect secrecy property
- Mathematical analysis requires no computational implementation
- Tags: perfect-secrecy, theoretical-foundations, one-time-pad, classic


## Hashing & Message Authentication

### 1. FIPS 202: SHA-3 Standard — NIST — 2015 — FIPS 202

- URL: http://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.202.pdf
- TL;DR: Official SHA-3 specification based on Keccak sponge construction, providing alternative to SHA-2 family.
- Significance: Latest NIST hash standard offering different security foundation from Merkle-Damgård construction.
- Reproducibility notes:
    - Code: [NIST reference](https://csrc.nist.gov/projects/cryptographic-standards-and-guidelines)
    - Data: test vectors provided
    - Replication difficulty: Moderate
  
Notes:

- Sponge construction enables extendable-output functions (XOFs)
- Reference implementation and extensive test vectors available
- Tags: sha-3, keccak, sponge-construction, nist-standard

### 2. HMAC: Keyed-Hashing for Message Authentication — Hugo Krawczyk, Mihir Bellare, Ran Canetti — 1997 — RFC 2104
- URL: https://tools.ietf.org/html/rfc2104
- TL;DR: Defines HMAC construction for message authentication using cryptographic hash functions with secret keys.
- Significance: Standard approach for message authentication, proven secure and widely implemented.
- Reproducibility notes:
    - Code: [Reference implementations](https://github.com/topics/hmac)
    - Data: test vectors in RFC
    - Replication difficulty: Easy

Notes:

- Simple construction easily implemented from specification
- Security proof demonstrates resistance to length-extension attacks
- Tags: mac, authentication, rfc, proven-secure


## Secret-key / Symmetric Cryptography

### 1. Advanced Encryption Standard (AES) — NIST — 2001 — FIPS 197
- URL: https://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.197.pdf
- TL;DR: Official specification of Rijndael as AES, defining 128/192/256-bit key variants of the US encryption standard.
- Significance: Most widely deployed symmetric cipher worldwide, with extensive hardware and software optimization.
- Reproducibility notes:
  - Code: [NIST reference](https://csrc.nist.gov/projects/cryptographic-algorithm-validation-program)
  - Data: test vectors provided
  - Replication difficulty: Easy

Notes:

- Complete test vector suites available for all key lengths
- Hardware implementations widely available for performance comparison
- Tags: block-cipher, standard, aes, nist

### 2. The Salsa20 Family of Stream Ciphers — Daniel J. Bernstein — 2007 — Various Publications
- URL: https://cr.yp.to/snuffle/salsafamily-20071225.pdf
- TL;DR: Describes Salsa20 stream cipher family emphasizing speed, security, and simplicity with ARX operations.
- Significance: Influenced modern stream cipher design and led to ChaCha20 adoption in major protocols.
- Reproducibility notes:
    - Code: [eSTREAM reference](https://cr.yp.to/streamciphers.html)
    - Data: test vectors
    - Replication difficulty: Easy
Notes:

Simple ARX-based design enables efficient software implementation
Extensive cryptanalysis shows strong security margins
Tags: stream-cipher, salsa20, arx-design, estream



### 3. ChaCha20-Poly1305 Cipher Suites for TLS — Adam Langley, et al. — 2016 — RFC 7905
- URL: https://tools.ietf.org/html/rfc7905
- TL;DR: Specifies ChaCha20 stream cipher with Poly1305 MAC for TLS, offering alternative to AES-GCM.
- Significance: Provides TLS performance benefits on mobile devices and demonstrates AEAD deployment.
- Reproducibility notes:
    - Code: [Multiple TLS libraries](https://github.com/topics/chacha20)
    - Data: test vectors in RFC
    - Replication difficulty: Moderate

Notes:

- Designed for software efficiency without AES hardware acceleration
- Real-world deployment data available from major browsers
- Tags: tls, chacha20, poly1305, aead

### 4. The Galois/Counter Mode of Operation (GCM) — David A. McGrew, John Viega — 2004 — Various

- URL: https://web.archive.org/web/20221007191258/https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.694.695&rep=rep1&type=pdf
- TL;DR: Introduces GCM authenticated encryption mode combining CTR encryption with GHASH authentication.
- Significance: Widely adopted AEAD mode providing both confidentiality and authenticity efficiently.
- Reproducibility notes:
    - Code: [OpenSSL implementation](https://github.com/openssl/openssl)
    - Data: test vectors available
    - Replication difficulty: Moderate

Notes:

- Parallelizable design enables high-speed implementations
- Requires careful nonce management to prevent catastrophic failures
- Tags: aead, gcm, authenticated-encryption, performance

## Cryptanalysis & Attacks

### 1. Timing Attacks on Implementations of Diffie-Hellman, RSA, DSS — Paul Kocher — 1996 — CRYPTO
- DOI: 10.1007/3-540-68697-5_9
- TL;DR: Demonstrates how timing variations in cryptographic implementations leak secret key information through side channels.
- Significance: Founded side-channel cryptanalysis field, showing implementation details critically affect security.
- Reproducibility notes:
    - Code: [Educational implementations](https://github.com/topics/timing-attack)
    - Data: none found
    - Replication difficulty: Hard

Notes:

- Requires precise timing measurement setup and statistical analysis
- Attack effectiveness highly dependent on target platform characteristics
- Tags: side-channel, timing-attack, implementation, practical


### 2. Cache Timing Attacks on AES — Daniel J. Bernstein — 2005 — Various
- URL: http://cr.yp.to/antiforgery/cachetiming-20050414.pdf
- TL;DR: Demonstrates practical cache-based side-channel attacks against table-based AES implementations.
- Significance: Shows that CPU cache behavior can leak cryptographic keys in real systems.
- Reproducibility notes:
    - Code: [Demo implementations](https://github.com/topics/cache-attack)
    - Data: none found
    - Replication difficulty: Hard

Notes:

- Requires detailed understanding of target CPU cache architecture
- Attack success depends on system load and measurement precision
- Tags: cache-attack, side-channel, aes, practical


### 3. Self-Study Course in Block Cipher Cryptanalysis — Bruce Schneier — 2000 — AES Candidate Conference
- URL: https://www.schneier.com/academic/archives/2000/01/self-study_course_in.html
- TL;DR: Systematic introduction to block cipher cryptanalysis techniques organized for self-directed learning.
- Significance: Influential educational resource for learning practical cryptanalytic methods and approaches.
- Reproducibility notes:
    - Code: none found
    - Data: example problems provided
    - Replication difficulty: Moderate

Notes:

Structured approach covers differential, linear, and related-key attacks
Includes practical exercises for developing cryptanalytic skills
Tags: cryptanalysis, educational, block-cipher, methodology


## Public-key Cryptography & DLP

### 1. New Directions in Cryptography — Whitfield Diffie, Martin Hellman — 1976 — IEEE Transactions on Information Theory
- DOI: 10.1109/TIT.1976.1055638
- TL;DR: Introduces public-key cryptography concept and Diffie-Hellman key exchange, revolutionizing secure communication.
- Significance: Launched modern cryptography era, enabling secure communication without prior shared secrets.
- Reproducibility notes:
    - Code: [Multiple implementations](https://github.com/topics/diffie-hellman)
    - Data: none needed
    - Replication difficulty: Easy

Notes:

- Algorithm simple enough to implement from paper description
- Numerous pedagogical implementations available across languages
- Tags: public-key, key-exchange, foundations, classic


### 2. A Method for Obtaining Digital Signatures and Public-Key Cryptosystems — Ronald Rivest, Adi Shamir, Leonard Adleman — 1978 — Communications of the ACM
- DOI: 10.1145/359340.359342
- TL;DR: Introduces RSA public-key cryptosystem based on integer factorization difficulty, first practical public-key scheme.
- Significance: First widely adopted public-key cryptosystem, still fundamental to internet security infrastructure.
- Reproducibility notes:
    - Code: [Multiple implementations](https://github.com/topics/rsa)
    - Data: none needed
    - Replication difficulty: Easy

Notes:

- Algorithm description sufficient for straightforward implementation
- Security depends critically on proper padding schemes (OAEP, PSS)
- Tags: public-key, rsa, classic, factorization

### 3. Twenty Years of Attacks on the RSA Cryptosystem — Dan Boneh — 1999 — Notices of the AMS
- URL: http://crypto.stanford.edu/~dabo/pubs/papers/RSA-survey.pdf
- TL;DR: Comprehensive survey of RSA attacks including mathematical, implementation, and protocol-level vulnerabilities.
- Significance: Essential reference for understanding RSA security analysis and implementation pitfalls.
- Reproducibility notes:
    - Code: none found
    - Data: attack examples
    - Replication difficulty: Moderate

Notes:

- Covers both theoretical attacks and practical implementation vulnerabilities
- Includes timing attacks and fault injection techniques
- Tags: rsa, survey, attacks, comprehensive


### 4. Remote Timing Attacks are Practical — David Brumley, Dan Boneh — 2003 — USENIX Security
- URL: http://crypto.stanford.edu/~dabo/papers/ssl-timing.pdf
- TL;DR: Demonstrates feasibility of timing attacks over networks against SSL/TLS implementations.
- Significance: Shows that side-channel attacks work in realistic network conditions, not just laboratory settings.
- Reproducibility notes:
    - Code: [Attack tools](https://github.com/topics/ssl-timing)
    - Data: measurement data
    - Replication difficulty: Hard

Notes:

- Requires network measurement tools and statistical analysis
- Attack effectiveness varies with network conditions and implementations
- Tags: timing-attack, ssl, network, practical


## Elliptic Curve Cryptography

### 1. Curve25519: New Diffie-Hellman Speed Records — Daniel Bernstein — 2006 — PKC
- DOI: 10.1007/11745853_14
- TL;DR: Presents Curve25519 elliptic curve designed for high-speed, secure Diffie-Hellman key exchange with built-in side-channel protection.
- Significance: Demonstrates that careful curve choice enables both performance and security, widely adopted in modern protocols.
- Reproducibility notes:
    - Code: [Reference implementation](https://cr.yp.to/ecdh.html)
    - Data: performance benchmarks
    - Replication difficulty: Moderate

Notes:

- Highly optimized assembly implementation achieves record performance
- Curve design prioritizes implementation security over mathematical elegance
-   Tags: elliptic-curve, diffie-hellman, performance, side-channel-resistant


### 2. High-Speed High-Security Signatures — Daniel Bernstein, et al. — 2011 — CHES
- URL: https://ed25519.cr.yp.to/ed25519-20110926.pdf
- TL;DR: Presents Ed25519 signature scheme using Edwards curves with deterministic signing and strong security properties.
- Significance: Demonstrates superior performance and security compared to ECDSA, avoiding nonce vulnerabilities.
- Reproducibility notes: 
    - Code: Reference implementation
    - Data: benchmark data
    - Replication difficulty: Moderate

Notes:

- Deterministic design eliminates catastrophic failures from poor randomness
- Complete verification and batch verification implementations available
- Tags: digital-signature, ed25519, edwards-curve, deterministic

### 3. Biased Nonce Sense: Lattice Attacks against Weak ECDSA Signatures — Joachim Breitner, Nadia Heninger — 2019 — IEEE S&P
- URL: https://eprint.iacr.org/2019/023.pdf
- TL;DR: Demonstrates recovery of ECDSA private keys by exploiting biased nonce generation in cryptocurrency implementations.
- Significance: Shows real-world impact of poor randomness in deployed cryptographic systems.
- Reproducibility notes:
    - Code: Attack implementation
    - Data: blockchain transaction data
    - Replication difficulty: Moderate

Notes:

- Requires blockchain data analysis and lattice reduction tools
- Demonstrates importance of proper random number generation
- Tags: ecdsa, nonce-bias, lattice-attack, cryptocurrency

## Zero-Knowledge Proofs

### 1. The Knowledge Complexity of Interactive Proof Systems — Shafi Goldwasser, Silvio Micali, Charles Rackoff — 1989 — SIAM Journal on Computing
- DOI: 10.1137/0218012
- TL;DR: Formalizes zero-knowledge proofs, showing how to prove statement knowledge without revealing the knowledge itself.
- Significance: Theoretical foundation for zero-knowledge protocols, enabling privacy-preserving verification systems.
- Reproducibility notes:
    - Code: none found
    - Data: none found
    - Replication difficulty: Hard

Notes:

- Highly theoretical work requiring deep complexity theory background
- Implementation requires translating abstract protocols to concrete constructions
- Tags: zero-knowledge, complexity-theory, foundations, theoretical

### 2. On the Size of Pairing-Based Non-interactive Arguments — Jens Groth — 2016 — EUROCRYPT
- DOI: 10.1007/978-3-662-49896-5_11
- TL;DR: Presents Groth16 zk-SNARK construction achieving constant-size proofs and efficient verification for general circuits.
- Significance: Enables practical zero-knowledge applications with minimal proof sizes, powering blockchain privacy systems.
- Reproducibility notes:
    - Code: libsnark implementation
    - Data: circuit examples
    - Replication difficulty: Hard

Notes:

- Requires trusted setup ceremony for each circuit
- Implementation demands expertise in pairing-friendly elliptic curves
- Tags: zk-snark, pairing-based, constant-size, practical

### 3. Bulletproofs: Short Proofs for Confidential Transactions — Benedikt Bünz, et al. — 2018 — IEEE S&P
- DOI: 10.1109/SP.2018.00020
- TL;DR: Non-interactive zero-knowledge proofs with logarithmic size and no trusted setup, suitable for range proofs.
- Significance: Removes trusted setup requirement while maintaining short proofs, adopted in cryptocurrency privacy protocols.
- Reproducibility notes:
    - Code: Reference implementation
    - Data: benchmarking data
    - Replication difficulty: Moderate

Notes:

- Rust implementation provides clean, well-documented reference
- Verification time grows with proof complexity unlike Groth16
- Tags: bulletproofs, no-trusted-setup, range-proof, cryptocurrency

## Post-Quantum Cryptography

### CRYSTALS-Kyber: Algorithm Specifications — Roberto Avanzi, et al. — 2020 — NIST PQC
- URL: https://pq-crystals.org/kyber/
- TL;DR: Lattice-based key encapsulation mechanism selected as NIST post-quantum cryptography standard for key establishment.
- Significance: Primary post-quantum KEM standard, preparing cryptographic infrastructure for quantum computing threats.
- Reproducibility notes:
    - Code: Reference implementation
    - Data: NIST test vectors
    - Replication difficulty: Moderate

Notes:

- NIST provides comprehensive test vectors for all parameter sets
- Multiple optimized implementations available for different platforms
- Tags: post-quantum, lattice-based, kem, nist-standard


### 2. CRYSTALS-Dilithium: Algorithm Specifications — Léo Ducas, et al. — 2018 — NIST PQC
- URL: https://pq-crystals.org/dilithium/
- TL;DR: Lattice-based digital signature scheme selected as NIST post-quantum standard offering strong security and efficiency.
- Significance: Primary post-quantum signature standard, enabling long-term digital signature security against quantum attacks.
- Reproducibility notes:
    - Code: [Reference implementation](https://github.com/pq-crystals/dilithium)
    - Data: NIST test vectors
    - Replication difficulty: Moderate

Notes:

- Modular design supports multiple security levels (Dilithium2/3/5)
- Implementations optimized for both software and hardware deployment
- Tags: post-quantum, lattice-based, digital-signature, nist-standard

### 3. Post-Quantum Cryptography — Daniel J. Bernstein, Johannes Buchmann, Erik Dahmen (eds.) — 2009 — Springer
- URL: https://eprint.iacr.org/2017/314.pdf (related survey)
- TL;DR: Comprehensive survey of mathematical approaches to cryptography resistant to quantum computer attacks.
- Significance: Foundational reference for understanding post-quantum cryptographic approaches and their trade-offs.
- Reproducibility notes:
    - Code: various implementations
    - Data: none needed
    - Replication difficulty: Moderate
Notes:

- Covers lattice-based, code-based, multivariate, and hash-based approaches
- Extensive bibliography and comparison of different approaches
- Tags: post-quantum, survey, comprehensive, quantum-resistance

## Key Management & Protocols

### 1. The Networking and Cryptography Library (NaCl) — Daniel Bernstein, et al. — 2012 — Various Publications
- URL: https://nacl.cr.yp.to/
- TL;DR: High-level cryptographic library providing simple APIs for authenticated encryption, signatures, and key exchange.
- Significance: Demonstrates secure-by-default cryptographic design, influencing modern library architecture and protocol selection.
- Reproducibility notes:
    - Code: [Reference implementation](https://nacl.cr.yp.to/install.html)
    - Data: test vectors
    - Replication difficulty: Easy

Notes:

- Complete working library with extensive testing and benchmarking
- Design philosophy prioritizes security over backwards compatibility
- Tags: cryptographic-library, secure-by-default, authenticated-encryption, practical


### 2. The Double Ratchet Algorithm — Trevor Perrin, Moxie Marlinspike — 2016 — Signal Specification
- URL: https://signal.org/docs/specifications/doubleratchet/
- TL;DR: Forward-secure messaging protocol providing confidentiality, authenticity, and perfect forward secrecy for asynchronous communication.
- Significance: Powers Signal and WhatsApp end-to-end encryption, demonstrating practical advanced cryptographic protocol deployment.
- Reproducibility notes:
    - Code: [libsignal implementation](https://github.com/signalapp/libsignal)
    - Data: test vectors
    - Replication difficulty: Moderate

Notes:

- Production implementation demonstrates real-world cryptographic protocol complexity
- Specification includes detailed security analysis and attack considerations
- Tags: messaging-protocol, forward-secrecy, signal, practical

### 3. Recommendation for Key Management — NIST — 2020 — NIST SP 800-57 Part 1
- URL: http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-57pt1r5.pdf
- TL;DR: Comprehensive guidance on cryptographic key management including generation, distribution, storage, and destruction.
- Significance: Authoritative reference for implementing secure key management in operational systems.
- Reproducibility notes:
    - Code: none found
    - Data: none needed
    - Replication difficulty: Easy

Notes:

- Covers key lifecycle management and algorithm selection guidance
- Regular updates reflect current cryptographic best practices
- Tags: key-management, nist, guidelines, operational

## Applied Systems & Standards

### TLS 1.3 — Eric Rescorla — 2018 — RFC 8446

- URL: https://tools.ietf.org/html/rfc8446
- TL;DR: Latest Transport Layer Security protocol removing legacy cryptography and improving security and performance.
- Significance: Foundation of internet security, demonstrating evolution toward modern cryptographic best practices.
- Reproducibility notes:
    - Code: [Multiple implementations](https://github.com/topics/tls13)
    - Data: test vectors
    - Replication difficulty: Hard

Notes:

- Complex protocol with multiple interacting cryptographic components
- Extensive test suites available for interoperability validation
- Tags: tls, internet-security, protocol, complex


## Reproducibility checklist

- License verification: Check code licensing terms and commercial usage restrictions before implementation
- Environment setup: Use specified compilers, library versions, and operating system configurations when provided
- Hardware requirements: Verify computational resources, especially for timing-sensitive cryptanalytic attacks
- Randomness handling: Use identical random seeds or understand impact of randomness on reproducible results
- Dataset access: Confirm availability of evaluation datasets and preprocessing steps described in papers
- Evaluation scripts: Locate and execute provided benchmarking and testing scripts to validate implementations
- Metric definitions: Understand security parameter choices, performance measurement methodologies, and success criteria
- Baseline comparisons: Implement or locate comparison algorithms using identical test conditions and parameters
- Statistical significance: Apply appropriate statistical methods for cryptanalytic success rates and performance measurements
- Citation practices: Properly attribute original authors and note any third-party implementations or modifications used

## Books & extended resources

### 1. A Graduate Course in Applied Cryptography — Dan Boneh, Victor Shoup — 2020
- URL: https://crypto.stanford.edu/~dabo/cryptobook/ (free online)
- TL;DR: Comprehensive modern cryptography textbook balancing theory and practice with rigorous security analysis.
- Significance: Leading graduate-level resource with freely available content and regular updates.
- Tags: textbook, applied-crypto, comprehensive, free

### 2. Handbook of Applied Cryptography — Alfred J. Menezes, Paul C. van Oorschot, Scott A. Vanstone — 1996
- URL: https://cacr.uwaterloo.ca/hac/ (free online)
- TL;DR: Classical comprehensive reference covering cryptographic algorithms, protocols, and implementation considerations.
- Significance: Standard reference text providing detailed algorithm descriptions and security analysis.
- Tags: handbook, comprehensive, classical, algorithms

### 3. The Joy of Cryptography — Mike Rosulek — 2021
- URL: http://web.engr.oregonstate.edu/~rosulekm/crypto/ (free online)
- TL;DR: Accessible introduction to modern cryptography with emphasis on provable security and practical understanding.
- Significance: Bridges gap between introductory and advanced treatments with clear explanations.
- Tags: textbook, accessible, provable-security, modern

## Online challenges & learning resources

### 1. CryptoHack 
- URL: https://cryptohack.org/
- Interactive cryptography challenges covering various topics from basic concepts to advanced attacks with hands-on learning approach.

### 2. Cryptopals Crypto Challenges

- URL: https://cryptopals.com/
- Progressive set of practical cryptography challenges demonstrating real-world attacks and implementation vulnerabilities.

### 3. Mystery Twister C3

- URL: https://www.mysterytwisterc3.org/en/
- Cipher contest with 200+ challenges of different difficulty levels, moderated forum, and hall-of-fame for competitive cryptanalysis learning.

### 4. id0-rsa Crypto Challenges

- URL: https://id0-rsa.pub/
- Advanced cryptographic challenges focusing on real-world attack scenarios and modern cryptographic primitives.

## Educational courses & lectures

- [Introduction to Cryptography — Christof Paar — University of Bochum](https://www.youtube.com/watch?v=2aHkqB2-46k): Comprehensive video lecture series covering cryptographic fundamentals with practical examples and clear explanations.
- [Cryptography I & II — Dan Boneh — Stanford/Coursera](https://www.coursera.org/learn/crypto): High-quality online courses covering modern cryptography theory and applications with programming assignments.
- [Crypto101 — Laurens Van Houtven](https://www.crypto101.io/): Introductory cryptography course designed for programmers of all skill levels with practical implementation focus.

## References & source notes
This bibliography was curated from multiple high-quality sources including the original Awesome Crypto Papers collection by pFarb, canonical cryptographic literature databases (ACM Digital Library, IEEE Xplore, IACR eprint archive, arXiv), and implementation repositories from GitHub and official standards bodies (NIST, IETF). Selection prioritized papers with demonstrated impact through citation counts, practical adoption, and availability of reproducible artifacts. The collection balances foundational theoretical contributions with modern practical systems to serve both academic researchers and implementation practitioners.

## Disclaimer
Annotations and reproducibility assessments represent approximate judgments based on publicly available information at the time of review. Readers should consult original papers, verify code licenses, and contact authors for authoritative implementation details. Security assessments reflect the state of knowledge at publication time and may not account for subsequent cryptanalytic developments or implementation vulnerabilities. Always verify cryptographic implementations through appropriate security review processes before production deployment. This list is educational in nature and not intended as implementation guidance for production systems without proper cryptographic review.

## License

This resource is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). Content is for educational and informational purposes only. Always consult qualified legal counsel for specific compliance requirements.

Regulatory requirements change frequently. Verify current requirements with appropriate authorities. Contributors are not responsible for the accuracy, completeness, or currency of external resources.

- Last Updated: August 27, 2025
- Maintainer: cryptowithshashisupport@gmail.com
- Contributors: 0









































