# Domain Name Signature Provider (DNSP)

The **Domain Name Signature Provider (DNSP)** is a program designed to verify and establish trust for domain owners by linking their domain name to a cryptographic key pair. It ensures that the domain owner is authenticated and can securely sign digital documents or data. The DNSP service operates in conformance with the [did:web Method Specification](https://w3c-ccg.github.io/did-method-web/) and the [High Assurance DIDs with DNS Guidance](https://www.ietf.org/archive/id/draft-carter-high-assurance-dids-with-dns-06.html) providing a decentralized and standardized approach for associating cryptographic credentials with domain names.

This is a program to enable mutual recognition of those who have successfully implemented the requirements outlined in [DEC-02 Sign and Verify With My Domain](dec-02.md)

## Key Features:

1. **Domain Ownership Verification**:
   - The service verifies that the user controls the domain name by requiring proof, such as updating DNS records or serving a specific file at a URL under the domain.
   - Once verified, the domain is associated with a public-private key pair.

2. **Public Key Resolution via DID Web**:
   - The public key is published in a standardized way using the W3C DID Web specification. This enables anyone to resolve the domain's public key by querying its DID Document, typically hosted at `https://<domain>/.well-known/did.json`.

3. **Secure Private Key Management**:
   - The private key is stored in a highly secure environment, such as a hardware security module (HSM) or equivalent secure enclave.
   - The private key is never exposed to the user or external systems, reducing the risk of unauthorized access or misuse.

4. **Digital Signature Service**:
   - The domain owner can use the service to sign documents, data, or transactions. This establishes a clear and verifiable link between the domain and the signed material.
   - Signatures are generated using the private key associated with the domain, ensuring authenticity and integrity.

5. **Interoperability and Decentralization**:
   - The service adheres to W3C DID standards, ensuring interoperability with other decentralized systems and identity frameworks.
   - Verifiers can use existing W3C DID resolvers to retrieve the domain's public key and validate signatures, making the system broadly compatible.

6. **Use Cases**:
   - **Secure Communications**: Ensure that messages or transactions purportedly from a domain are genuine.
   - **Document Signing**: Sign contracts, agreements, or other documents with cryptographic proof linked to a domain.
   - **Web of Trust**: Establish a decentralized trust mechanism by linking domain ownership to cryptographic identities.

## Benefits:

- **Trust and Transparency**: Provides cryptographic proof that a domain owner has signed the data.
- **Security**: Protects the private key from compromise, ensuring that only the verified domain owner can generate signatures.
- **Standardization**: Leverages globally recognized W3C standards for broad compatibility and trustworthiness.
- **Decentralized Verification**: Allows anyone to independently verify domain signatures without relying on centralized authorities.

The Domain Name Signature Provider Program thus enables domain owners to securely participate in decentralized trust networks, empowering them with tools to establish authenticity and credibility in the digital world.