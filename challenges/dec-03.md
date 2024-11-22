# Domain Name Signature Provider (DNSP) Program

This digital ecosystem challenge aims to establish a **Domain Name Signature Provider (DNSP)** program that is designed to verify and establish trust for domain owners by linking their domain name to a cryptographic key pair. The program ensures that the domain owner is verified and demonstrates the capability to securely sign digital documents or data. 

This challenge builds on those who have implemented [DEC-02 Sign and Verify With My Domain](dec-02.md) and who wish to be formally recognized for their investment in building stronger digital ecosystem.

## Core Conformance Requirements
The DNSP program is intended to operate in conformance with the [did:web Method Specification](https://w3c-ccg.github.io/did-method-web/) and the [High Assurance DIDs with DNS Guidance](https://www.ietf.org/archive/id/draft-carter-high-assurance-dids-with-dns-06.html). 

## Supplementary Conformance Requirements
For higher assurance level requirements and sector-specific requirements the following national standards and specifications may be applied:
- [DGSI/TS 115 Technical Specification for Digital Credentials and Digital Trust Services](https://dgc-cgn.org/standards/find-a-standard/standards-in-digital-credentials/digital-credentials/)
- [CAN/DGSI 103-0: Digital Trust & Identity - Part 0 - Techniques - Code of Practice](https://dgc-cgn.org/standards/find-a-standard/standards-in-digital-trust/can-ciosc-103-0-digital-trust-identity-part-0-techniques-code-of-practice/)
- [CAN/DGSI 103-1: Digital Trust & Identity – Part 1 – Fundamentals](https://dgc-cgn.org/standards/find-a-standard/standards-in-digital-trust/digital-trust-fundamentals/)
- [CAN/DGSI 103-2: Data Trust & Identity – Part 2 – Delivery of Healthcare Services](https://dgc-cgn.org/standards/find-a-standard/standards-in-digital-trust/digital-trust/)
- [CAN/DGSI 103-3: Digital Trust & Identity – Part 3 – Digital Credentials](https://dgc-cgn.org/standards/find-a-standard/standards-in-digital-trust/digital-credentials/)

## Verification
Verification would be conducted under the auspices of the [DGC Digital Trust Conformity Assessment Program](https://github.com/dgc-cgn/CAS-Digital-Trust).

## Program Outcome
The **program outcome** is confidence in the marketplace that a decentralized and standardized approach for verifying cryptographically signed documents and credentials using commonly known domain names can serve the needs of a broad array of users and stakeholders.

## Mutual Recognition
This is a program intended to enable mutual recognition of those who have successfully implemented the requirements and guidance outlined above and have undergone a formalized verification process.

## Key Features:
The program verifies the following.

1. **Domain Ownership Verification**:
   - The user controls the domain name by requiring proof, such as updating DNS records or serving a specific file at a URL under the domain.
   - Once verified, the domain is properly associated with a public-private key pair.

2. **Public Key Resolution via DID Web**:
   - The public key is published in a standardized way using the W3C DID Web specification. This enables anyone to resolve the domain's public key by querying its DID Document, typically hosted at `https://<domain>/.well-known/did.json`.

3. **Secure Private Key Management**:
   - The private key is stored in a secure environment, that may include a hardware security module (HSM) or equivalent secure enclave.
   - The private key is secure and not exposed to unauthorized users or external systems, reducing the risk of unauthorized access or misuse.

4. **Digital Signature Service**:
   - The domain owner can use the service to sign documents, data, or transactions. This establishes a clear and verifiable link between the domain and the signed material.
   - Signatures are generated using the private key associated with the domain, ensuring authenticity and integrity.

5. **Interoperability and Decentralization**:
   - The service adheres to W3C DID standards, ensuring interoperability with other decentralized systems and identity frameworks.
   - Any verifiers can use existing W3C DID resolvers or implement their own to retrieve the domain's public key and validate signatures, making the system broadly compatible.

## Use Cases:
   - **Secure Communications**: Ensure that messages or transactions purportedly from a domain are genuine.
   - **Document Signing**: Sign contracts, agreements, or other documents with cryptographic proof linked to a domain.
   - **Web of Trust**: Establish a decentralized trust mechanism by linking domain ownership to cryptographic identities.

## Benefits:
- **Trust and Transparency**: Provides cryptographic proof that a domain owner has signed the data.
- **Security**: Protects the private key from compromise, ensuring that only the verified domain owner can generate signatures.
- **Standardization**: Leverages globally recognized W3C standards for broad compatibility and trustworthiness.
- **Decentralized Verification**: Allows anyone to independently verify domain signatures without relying on centralized authorities.

## Strategic Outcome

The **Domain Name Signature Provider Program** enables trust and confidence in domain owners who have been verifed to enable secure participation in decentralized trust networks, empowering users, service providers and the broader digital ecosystem of stakeholders with tools to establish authenticity, credibility and verifiability in the digital world.