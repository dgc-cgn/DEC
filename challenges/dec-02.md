# DEC-02 Sign and Verify With My Domain
[French](./dec-02-fr.md)
## Overview

A compelling use of the new WC3 Decentralized Identifiers (W3C DIDs) is to enable the capability to “sign and verify with my domain”. Simply put, your domain, your website - something that is already well-known to your users - becomes a trusted identifier you can use to sign anything you want to be verified.

“Sign and verify with my domain” provides an immediate benefit to website owners who can leverage their existing domain name registrars and certificated authorities (CAs) to enable the implementation of trusted identifiers. This approach is open and non-proprietary; it works regardless of whether the signing authority is a government organization, a commercial enterprise, or an individual. To sum up, it works for everyone because the approach embraces the open web.

A key enabler is the Decentralized Identifier or DID. A DID is a new component standardized by the World Wide Web Consortium (W3C). A DID is a type of URI that is globally unique, highly available, and cryptographically verifiable with no required central authority. DIDs can be associated with an entity (DID Subject) by means of metadata describing the entity (contained within DID Document) and how to interact with it. This challenge leverages a specific method: `did:web` that enables an association with a domain name and its owner.


## Expected Outcomes

1. A working implementation in accordance with the High Assurance DIDS with DNS. In simple terms, a website domain having the address of `https://example.com` should be able to sign documents with the correspond DID `did:web:example.com`.
2. The ability to verify a document (pdf) or verifiable credential using the High Assurance DID, for example `did:web:example.com`

## Participation

We are looking for participants who are willing be a part of a cohort to demonstrate. Participants can be issuers, verifiers, or most importantly, holders who require the authenticity of documents to be confirmed.

### Current Partipants

|Organization|Contact(s)|Primary Interest(s)|
|---|---|---|
|Digital Governance Council|Tim Bouma|Convenor, Standards|
|CIRA| Jacques Latour, Jesse Carter|Infrastructure, Standards|
|Northern Block|Mathieu Glaude|Commercial Vendor|


## Helpful Diagrams

A couple of helpful diagrams below. The full briefing can be found [here](./pubs/HIADID-Briefing.pdf)

![](./assets/HIADID.png)
![](./assets/VCHIADID.png)

## Key References

* High Assurance DIDS with DNS [IETF Draft RFC](https://www.ietf.org/archive/id/draft-carter-high-assurance-dids-with-dns-05.html)
