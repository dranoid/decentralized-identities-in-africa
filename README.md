# Decentralized Identities and Why They Are Important in Africa

It is estimated that in Sub-Saharan Africa, about 500 million people lack a means of legal identification. This limits their access to financial services, makes the process of social welfare reaching these people more difficult and less transparent, reduces the quality of healthcare available to them as it will be difficult to maintain a medical record without an identity to tie it to and also limits access to quality education. In this article, we are going to be exploring what decentralized identities are, how they compare to centralized means of identity management, how they can help improve this situation, and also some of the limitations and challenges that are going to be faced in its implementation.

It goes without saying that the current identity management system in Africa is centralized, meaning that the issuance, verification, and even revocation of valid means of identification like passports, driving licenses, certificates, and employment IDs is done by a single or separate entity each responsible for the protection (to prevent data leaks) and safety (to prevent data loss) of their data. In countries in Africa where adoption of technology is lower than the global average, a lot of this data is usually kept as physical files onsite in the issuer’s offices. This is dangerous for a lot of reasons of which I will just mention a few, the risk of damage to the physical copies of records is high either due to fires or floods or even human error, and the physical records are also extremely inefficient when compared to the digitally kept records. The digital records too are not fully safe as evidenced by data breaches that affected technological giants like Facebook, Yahoo, and Atlassian amongst others in the past and duplicates of the same information about an individual make it easier for a mistake to occur in one of the instances, I have been a victim of this. Another notable mention is the forgery of certificates which is a pressing issue in Africa, especially in Nigeria as most people don’t usually go through the hassle of trying to verify a certificate, or even if they are ready to go through that hassle, the process is frustrated by the slow or non-coming responses from the issuer. Decentralized Identities, while not a one-size-fits-all solution, addresses most of these problems.

## What is a Decentralized Identity?

In simple terms, decentralized identity management is where a user is in control of their digital identity without depending on a specific service provider. Leveraging the blockchain (or similar) technology and cryptographic keys to make the information verifiable and tamper-proof, decentralized identities allow a user to release only the important or necessary information to whatever service requires it, an example is a service that needs to confirm if you are above the age of 18, there’s no need for the service to be aware of your date of birth, decentralized identities make it possible to just specify which data is released to what service.

## How Does It Work?

Before we dive into how decentralized identities work, let’s define the entities or parties in a transaction (all the steps from issuing to verifying the certificates).

1. **Issuer**: Firstly we have the Issuer, which as the name states, is any body or institution that can issue a certificate ascertaining a fact about you or credentials that describe you.
2. **Credentials**: Credentials are claims that the issuer makes about you, they can be anything from your work ID card to your driver’s license or your school certificate as long as it is a document that can be used to identify you or verify your involvement with the issuer it is a credential.
3. **Verifiers**: Verifiers are entities that ensure that an issued credential is valid, think of them like those bouncers at concerts that check for tickets, another example is a gym verifying your health insurance claim before you are offered a membership discount.
4. **Verifiable Credential**: Another term to define is something called a Verifiable Credential which are tamper-evident claims that can be cryptographically verified, and include proof of who issued it. A verifiable credential includes claims about the subject, metadata, and cryptographic proofs. Verifiable credentials also often contain decentralized identifiers (DIDs) which is a fundamental building block that resolves or points to a DID document on the blockchain that holds information such as a set of data describing the DID subject, including mechanisms, such as cryptographic public keys, that the DID subject or a DID delegate can use to authenticate itself and prove its association with the DID (basically the public key is used to authenticate the identity of whoever owns the DID).

To understand how decentralized identities work it is important to note once again that there is no location where all the information of all the users with access to an entity’s services is stored all the information is held by their respective users and is shared on a need-to-know basis. 
Central to this is the user’s wallet, which is a digital app that holds the private keys relating to the information stored there. 
Decentralized identities use a pair of public (shared on the DID document) and private cryptographic keys (secured and usually kept in the user’s wallet as earlier described). Standards for the creation and use of DIDs are specified in the **W3C DID Core Specification**.

### Workflow Example

I’ve shown the different parts and what they do, this is the workflow for a ‘transaction’ that incorporates everything we’ve just discussed
A Verifiable Credential containing certain claims and an Issuer DID and a subject DID is Issued by Entity A (issuer) about Entity or Individual B(user). Entity or Individual B wants to access a service from Entity C (verifier) that requires verification from Entity A., Entity or Individual B presents the Verifiable Credentials which contain the required claims for verification and the DIDs that identify and cryptographically authenticate Entity A (Issuer) and Entity or Individual B (User) ensuring the integrity (tamper-proof) and authenticity	of the credential.

## How are Decentralized Identities Important in Africa?

Now that we’ve seen what decentralized identities are and how they differ from centralized identity management systems let’s look at the impact they can have in Africa and why that is important.

1. **Fraud-Proof Certificates**: Unusually but importantly, I will start with Fraud-proof certificates. Using the immutability of blockchain, decentralized	identities will eliminate the use of forged certificates in Africa, as any attempted change in the certificate will be very obvious from the cryptographic hash.
2. **Financial Inclusion**: Currently the African tech ecosystem is still trying to bank the unbanked, potential users already having easily verifiable and secure identities making it easy for onboarding, KYC, and accessing credit.
3. **Government Services**: Transparent access to social welfare programs will be enabled by DIDs thereby benefitting the people who need it the most. An area of application I foresee DIDs excelling in is user voting as it ticks all the requirements to ensure a voting system is transparent and efficient 
4. **Healthcare Accessibility**: Having an identity to attach medical history to will improve the quality of healthcare for the people concerned and it will be easy to ‘move’ your history across medical institutions.
5. **Support for AfCFTA**: A potential use of decentralized identities I didn’t initially talk about when listing issues but is too important to leave out is easing things for the African countries participating in the African Continental Free Trade Area (AfCFTA) as proposed by the AU. If interoperable digitally decentralized identities are developed by these countries it will be a huge step in further smoothening the workings and goals of the AfCFTA. 

## Challenges in Implementation

As stated earlier decentralized identities are not a one-size-fits-all solution to identity management, here are some of the issues that will be faced in the integration or adoption in Africa.

- Technological and infrastructure barriers
- Regulatory, legal, and policy issues
- User adoption and trust

Decentralised identities if implemented in Africa look like it will play a promising role in the further development of the continent. As digital literacy and infrastructure improves, I expect adoption to increase.


## References

- [Decentralized identifier - Wikipedia](https://en.wikipedia.org/wiki/Decentralized_identifier)
- [Decentralized Identity: The Ultimate Guide 2024 (dock.io)](https://www.dock.io/post/decentralized-identity#decentralized-identity-and-self-sovereign-identity-whats-the-difference)
- [Beginner's Guide to Decentralized Identity | KuppingerCole](https://www.kuppingercole.com/insights/decentralized-identity/decentralized-identity-guide#heading1)
- [Digital ID systems in Africa: Challenges, risks and opportunities – ECDPM](https://ecdpm.org/work/digital-id-systems-africa-challenges-risks-and-opportunities#:~:text=Despite%20this%20progress%2C%20achieving%20universal,identification%20in%20Sub%2DSaharan%20Africa)
