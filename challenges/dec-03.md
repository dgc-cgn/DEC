# Let's Sign and Verify

A program to enable the widescale adoption of digital signing and verification of documents on the internet. 

This program is named after the inspirational success of [Let's Encrypt](https://letsencrypt.org/), a free service provided by the [Internet Security Research Group (ISRG)](https://www.abetterinternet.org/).

This program was originally entitled **Domain Name Signature Provider (DNSP) Program** but we'll use the better name **Let's Sign and Verify** if it can enable a better internet.

If you wish to participate or learn more, please contact [info@dgc-cgn.org](mailto:info@dgc-cgn.org)

## Overview 

### The Need for a Stronger Digital Ecosystem

There is a need to digitally sign and verify documents in a way that is open, inclusive and leverages the strength of the web infrastructure currently in place. Until now, it has been difficult, but with recent advances in standards and guidance, it is now possible for every website owner to add the ability to sign documents and enable verification with their domain name. Many website owners who are now implementing [DEC-02 Sign and Verify With My Domain](dec-02.md) now wish to be formally recognized for their investment in building stronger digital ecosystem.

### Establishing a Practical Program for Digital Trust

This digital ecosystem initiative aims to establish a **Domain Name Signature Provider (DNSP)** practical program that enable website owners to link their domain name to a cryptographic key that is used to verify documents that they issue. 

In practical terms, if a user receives a document signed by a website owner with a well-known domain name—such as agency.canada.ca—the document can be quickly verified by referencing the public key associated with agency.canada.ca. This combination of a recognized domain name and its corresponding public key ensures reliable confirmation that the document was signed by the legitimate issuer and remains untampered.

This program is intended ensures that the domain owner is a legitimate entity, can demonstrate the capability to securely sign digital documents, and enables easy verificiation of these documents.


No new technolgy is needed. The DNSP utilizes widely used web and infrastructure capabilities, enabling any website owner to issue authentic documents that are easy to verify, such as invoices, letters of enrollment, and proofs of income.


## Core Conformance Requirements

The initial DNSP program is intended to apply the following recommendations and guidance for the purposes of verification and mutual recognition: 

- [did:web Method Specification](https://w3c-ccg.github.io/did-method-web/) 
- [High Assurance DIDs with DNS Guidance](https://www.ietf.org/archive/id/draft-carter-high-assurance-dids-with-dns-06.html)


## Supplementary Conformance Requirements

For higher assurance level requirements and sector-specific requirements the following national standards and specifications may be applied for verification:
- [DGSI/TS 115 Technical Specification for Digital Credentials and Digital Trust Services](https://dgc-cgn.org/standards/find-a-standard/standards-in-digital-credentials/digital-credentials/)
- [CAN/DGSI 103-0: Digital Trust & Identity - Part 0 - Techniques - Code of Practice](https://dgc-cgn.org/standards/find-a-standard/standards-in-digital-trust/can-ciosc-103-0-digital-trust-identity-part-0-techniques-code-of-practice/)
- [CAN/DGSI 103-1: Digital Trust & Identity – Part 1 – Fundamentals](https://dgc-cgn.org/standards/find-a-standard/standards-in-digital-trust/digital-trust-fundamentals/)
- [CAN/DGSI 103-2: Data Trust & Identity – Part 2 – Delivery of Healthcare Services](https://dgc-cgn.org/standards/find-a-standard/standards-in-digital-trust/digital-trust/)
- [CAN/DGSI 103-3: Digital Trust & Identity – Part 3 – Digital Credentials](https://dgc-cgn.org/standards/find-a-standard/standards-in-digital-trust/digital-credentials/)

## Related Implementations

- **DHS Implementation the U.S. Department of Homeland Security’s (DHS)** strategic implementation of decentralized identity, focusing on trust architectures to support secure and scalable digital identity verification for public sector applications.
[DHS Trust Architecture](https://dhs-svip.github.io/requirements-for-decentralized-identity/TrustArchitecture/)
- **DIF Trust DID Web Decentralized Identity Foundation** initiative to develop standards and best practices for DID, promoting interoperable, web-based decentralized identities to enhance trust and usability across digital services.
[Trust DID Web - did:tdw](https://identity.foundation/trustdidweb/)

## Verification Methodology

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

## Strategic Outcomes

The **Domain Name Signature Provider Program** would enables trust and confidence in domain owners who have been verifed to enable secure participation in decentralized trust networks, empowering users, service providers and the broader digital ecosystem of stakeholders with tools to establish authenticity, credibility and verifiability in the digital world.



