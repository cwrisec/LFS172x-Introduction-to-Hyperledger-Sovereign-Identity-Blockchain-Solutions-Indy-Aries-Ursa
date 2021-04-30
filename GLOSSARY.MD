
# Glossary SSI - Self-Sovereign Identity - SSI
## Christophe Maertens

A

**Agent**
A software program or process used by or acting on behalf of an entity to interact with other agents or with the Sovrin Ledger or other distributed ledgers. Embedded within an agent is a Key Management Service (KMS) that performs cryptographic operations on behalf of the entity the agent represents.

**Agent Interface**
The agent interface is a component of an agent that allows the agent to establish and manage connections with other agents and exchange messages with those agents

B

C

**Claim**
An assertion about an attribute of a subject. Examples of a claim include date of birth, height, government ID number, or postal address—all of which are possible attributes of an individual. A credential is comprised of a set of claims.

**Controller**
A controller provides the rules that define what actions an agent will initiate and how the agent will respond to events. There is a controller for every agent instance.

**Credential**
A digital assertion containing a set of claims made by an entity about itself or another entity. A credential is based on a credential definition. Examples of credentials include college transcripts, driver licenses, health insurance cards, and building permits.

**Credential Definition (CredDef)**
A machine-readable definition of the semantic structure of a credential based on one or more schemas. Credential definitions are stored on the ledger. Credential definitions must include an issuer public key. Credential definitions facilitate interoperability of credentials and proofs across multiple issuers, holders, and verifiers.

D

**Decentralized Identifier (DID)**
A special kind of identifier that is created by its owner, independent of any central authority. It is a globally unique identifier developed specifically for decentralized systems as defined by the W3C DID specification. DIDs enable interoperable decentralized self-sovereign identity management. A DID is associated with exactly one DID Document.

**Decentralized Key Management Systems (DKMS)**
An approach to cryptographic key management where there is no central authority. DKMS leverages the security, immutability, availability, and resiliency properties of distributed ledgers to provide highly scalable key distribution, verification, and recovery.

**Device Authorization Registry**
A mechanism that has been prototyped in Indy that adds another step to the presentation of an Indy proof—proof that the agent on the device that created the proof is authorized to do so.

**DID Communication (DIDComm)**
A messaging communication mechanism secured using the keys and service endpoints stored within DIDs owned by the communicating parties.

**DIDComm Content Protocols**
Protocols that define back-and-forth sequences specific messages sent between collaborating agents to accomplish some shared goal. DIDComm Content Protocol messages are delivered in DIDComm Envelope Protocol messages.

**DIDComm Envelope Protocol**
The method by which DIDComm Content Protocol messages are delivered, irrespective of the message content. The content message is encrypted and stored within the envelope.

**DID Exchange Protocol**
The method by which connections are established between agents with different roles (inviter, invitee), using a sequence of message types (invitation, request, response) to exchange data elements (IDs, DIDs, DIDdocs). See the Aries Request for Change (RFC) specification of the DID Exchange protocol.

**DID Document**
The machine-readable document to which a DID points as defined by the W3C DID specification. A DID document describes the public keys, service endpoints, and other metadata associated with a DID. A DID document is associated with exactly one DID.

**DID Method**
A specification that defines a particular type of DID conforming to the W3C DID specification. A DID Method specifies both the format of the particular type of DID as well as the set of operations for creating, reading, updating, and deleting (revoking) it.

**Distributed Ledger Technology**
A distributed ledger (also called a shared ledger or distributed ledger technology or DLT) is a consensus of replicated, shared, and synchronized digital data geographically spread across multiple sites, countries, or institutions.[1] There is no central administrator or centralized data storage.

For the purposes of this course, we use the terms blockchain, ledger, decentralized ledger technology (DLT) and decentralized ledger (DL) interchangeably even though there are differences.

F

G

**Governance Framework**
The set of business, legal, and technical definitions, policies, specifications, and contracts by which the members of a trust community agree to be governed in order to achieve their desired levels of assurance. A governance framework is also known as a trust framework.

H

**Holder**
A role played by an entity when it is issued a credential by an issuer. The holder may or may not be the subject of the credential. (There are many use cases in which the holder is not the subject, e.g., a birth certificate where the subject is a baby and both the mother and father may be holders. Another case is a credential registry.) If the credential supports zero-knowledge proofs, the holder is also the prover. Based on the definition provided by the W3C Verifiable Claims Working Group.

**Hyperledger**
An initiative of the Linux Foundation to develop open source distributed ledger and blockchain technology.

**Hyperledger Aries**
Hyperledger Aries is infrastructure for blockchain-rooted, peer-to-peer interactions. It includes shared cryptographic storage for blockchain clients as well as a communications protocol for allowing off-ledger interaction between those clients. This project consumes the cryptographic support provided by Hyperledger Ursa, to provide secure secret management and decentralized key management functionality.

**Hyperledger Indy**
An open source project under the Hyperledger umbrella for decentralized self-sovereign identity. The source code for Hyperledger Indy was originally contributed to the Linux Foundation by the Sovrin Foundation. Sovrin stewards run the Hyperledger Indy node software to operate their nodes.

**Hyperledger Ursa**
Hyperledger Ursa is a shared cryptographic library that enables people (and projects) to avoid duplicating other cryptographic work and hopefully increase security in the process. The library is an opt-in repository for projects (and potentially others) to place and use crypto.

I

**Issuer**
The entity that issues a credential to a holder.

**Issuer Credential Protocol**
Is used to enable an issuer to provide a holder with a verifiable credential.

J

K

**Key Management Service (KMS)**
A software module, and optionally an associated hardware module, for securely storing and accessing private keys, link secrets, other sensitive cryptographic key material, and other private data used by an entity. A KMS is local to, and accessed by, an agent.

**Key Recovery**
The process of recovering access to and control of a set of private keys—or an entire wallet—after loss or compromise. Key recovery is a major focus of the emerging DKMS standard for cryptographic key management. See also Recovery Key.

L

**Ledger Interface**
The ledger interface enables reading and writing DIDs and other transactions to/from the ledger. It will likely consist of a: DID resolver, writing mechanism and verifiable credential handler.

**Link Secret**
An item of private data used by the prover to link a credential uniquely to the prover. A link secret is an input to zero-knowledge proofs (ZKPs) that enables claims from one or more credentials to be combined in order to prove that the credentials have a common holder (the prover). A link secret should be known only to the prover.

M

N

**NYM**
Short for “pseudonym” and an early name for what is now called a DID.

O

P

**Pairwise**
A direct relationship between exactly two entities. Business-to-business relationships are pairwise by default. A DID or a public key or a service endpoint is pairwise if it is used exclusively in a pairwise relationship.

**Plenum Byzantine Fault Tolerant Protocol**
Plenum is the heart of the distributed ledger technology inside Hyperledger Indy. As such, it provides features somewhat similar in scope to those found in Hyperledger Fabric.

**Pluggable**
A mechanism used in software that defines how a component is to be used, while allowing for different implementations (plugins) to be created and used. An example in Hyperledger Aries is the interface to secure storage for an agent is defined, but plugins for different databases (SQLite, Postgres) can be deployed in different Aries agent instances.

**Private Key**
The half of a cryptographic key pair designed to be kept as the private data of an entity. In elliptic curve cryptography, a private key is called a signing key.

**Proof**
Cryptographic verification of a claim or a credential. A digital signature is a simple form of proof. A cryptographic hash is also a form of proof. Zero-knowledge proofs enable selective disclosure of the information in a credential.

**Proof Request**
The data structure sent by a verifier to a holder that describes the proof required by the verifier.

**Prover**
A role played by an entity when it generates a zero-knowledge proof from a credential. The prover is also the holder of the credential.

**Public Key**
The half of a cryptographic key pair designed to be shared with other parties in order to decrypt or verify encrypted communications from an entity. In digital signature schemes, a public key is also called a verification key. A public key may be either public data or private data depending on the policies of the entity.

**Public DID**
A DID that is intended to be widely available—resolvable by anyone that is presented with the DID.

**Private DID**
A DID shared only between parties that will use the DID, usually just one other party (pairwise). Instead of publishing private DIDs on the blockchain for anyone in the world to see, entities create DIDs and DIDDocs and then send them directly to the other party(ies) to hold. No one other than the parties involved can see or resolve the DIDs.

Q

R

**Recovery Key**
A special private key used for purposes of recovering the data of an agent after loss or compromise. In the DKMS key management protocol, a recovery key may be cryptographically sharded for secret sharing among multiple trustees.

**Resolver**
A software module that accepts an identifier as input, looks up the identifier in a database or ledger, and returns metadata describing the identified entity. The Domain Name System (DNS) uses a DNS resolver. Self-sovereign identity uses a DID resolver.

**Revocation**
The act of an Issuer revoking the validity of a Claim or a Credential. With the Sovrin Protocol and the Sovrin Ledger, Revocation is accomplished using a Revocation Registry.

S

**Schema**
A machine-readable definition of the semantics of a data structure. Schemas are used to define the attributes used in one or more credential definitions.

**Selective Disclosure**
A privacy-by-design principle of revealing only the subset of the data described in a claim, credential, or other set of private data that is required by a verifier. There are many techniques for achieving selective disclosure. One of the primary techniques used in Hyperledger Indy is zero-knowledge proof cryptography.

**Self-Sovereign Identity**
Lifetime portable identity for any person, organization, or thing that does not depend on any centralized authority and can never be taken away..

**Service Endpoint**
An addressable network location offering a service operated on behalf of an entity. As defined in the DID specification, a service endpoint is expressed as a URI (Uniform Resource Identifier).

**Sovrin Foundation**
The non-profit public trust organization chartered to administer Sovrin Infrastructure on behalf of the Sovrin Community. The Sovrin Foundation is the Governance Authority for the Sovrin Governance Framework and the Sovrin Web of Trust Framework.

**SSI**
Acronym for Self-Sovereign Identity.

**Steward**
An organization approved by the Sovrin Foundation to operate a node. A steward must meet the qualifications defined in the Steward Business Policies and the technical requirements defined in the Steward Technical Policies.

T

**Transaction**
A record of any type written to the Sovrin Ledger.

**Transaction Author Agreement**
A controlled document that functions as a legal agreement between the Sovrin Foundation and any transaction author, which must be digitally signed or otherwise explicitly agreed to by the transaction author in order to write a transaction.

**Trust over IP (ToIP)**
ToIP is a set of protocols being developed to enable a layer of trust on the Internet, protocols embodied in Indy, Aries and Ursa. It includes self-sovereign identity in that it covers identity, but goes beyond that to cover any type of authentic data.

U

**Universal DID Resolver**
An online service that supports the resolution of all DID methods and that can be used to resolve a DID and return a result when it cannot be resolved locally.

V

**Verifiable Credential**
A credential that includes a proof from the issuer. Typically this proof is in the form of a digital signature.

**Verifier**
An entity who requests a credential or proof from a holder and verifies it in order to make a trust decision about an entity.

W

X

Y

Z

**Zero-Knowledge Proof**
A proof that uses special cryptography and a link secret to support selective disclosure of information about a set of claims from a set of credentials. A zero-knowledge proof provides cryptographic proof about some or all of the data in a set of credentials without revealing the actual data or any additional information, including the identity of the prover.