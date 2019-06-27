# Omnione Technical review (v1.0)

1. BlockChain

Our OmniOne block chain uses an algorithm that is modified from DPOS + aBFT to have a speed advantage. With a consensus model able to handle more than 2,000 transactions per second, it is possible to respond to DID Signature Verification, Verifiable Claim Issuance, and Claim Verification in real time. The Authentication-only OmniOne Platform can replace authentication solutions that based on existing centralized authentication or identity infrastructure with its blockchain infrastructure. Users benefit by getting rewarded OMN tokens as they use blockchain-based services for authentication and service registration.

The basic functions performed in the blockchain are DID management and processing for authentication, and are designed not to collect or rely upon any personal identity information of a User. In the ecosystem made possibly by the OmniOne Platform, an Issuer can leverage their existing KYC process to create an additional revenue stream by helping to provide infrastructure for authentication at a lower cost by issuing Verifiable Claims that can establish User identity. Service Providers that need authentication can take advantage of the service to meet their demand for user identification, without relying on creating and managing their own separate centralized identity store that exposes them to compliance and reputational risk owing to the constant threat of data breach.



![omniSW](https://github.com/OmniOne-Blockchain/Bahama_Demo/blob/master/img/omniSW.png)


2. Decentralized Identity and Identification using DID (Decentralized Identity Documents)

OmniOne is a block-chain based Decentralized identity Platform that aims to provide self-sovereign digital identity.

OmniOne's DID method specification (https://github.com/OmniOneID/did_method) is implemented based on the DID specification by the W3C and is stored on the Omni-blockchain. This dramatically reduces public key delivery problems.

The OmniOne DID is made up of JSON data that includes an ID and a public key, both of which can be stored on the blockchain to make it easy to see who is asserted when a DID Entity (User) makes a claim about its identity.

The blockchain contains the entire DID document per User ID. The DID document contains a decentralized ID and a set of public keys for that DID according to the DID specification.

User DID documents stored on the blockchain ledger are not modifiable or removable. This is a combination of blockchain and DID to create a identity security infrastructure that enables various types of identification and authentication based on DID.



3. Secure storage of DID private keys and FIDO

![img](https://lh3.googleusercontent.com/Hf3xDcxLRFZEGujG4Qlh_tMOcmAHdsafHHScKpdrvtX0icRTFmCC_dbSqEc-PnB_kgO0u2sXFsWChgZPp-akDkZ2cPU09mir9DU-cbWm5xZo_UypeBd6yY11QqEIDouyIQgBGw)

OmniOne provides a powerful security mechanism for devices when users use the Online Service or Web Service. OmniOne is designed to provide SSI with more robust security by delegating FIDO's biometric authentication to parts of private key management that the existing DID specification does not clearly demonstrate.

OmniOne ultimately has implemented dFIDO and enhances Identity Security by leveraging FIDO over the dPKI that DIDs create.



4. Verifiable Claims

![credential](https://www.w3.org/TR/verifiable-claims-data-model/diagrams/credential.svg)

Source: https://www.w3.org/TR/verifiable-claims-data-model/

A Verifiable Claim using DID is a claim that gives a specific qualification to a DID-based User on the OmniOne Platform. Developed in compliance with the W3C specification (https://www.w3.org/TR/verifiable-claims-data-model/), OmniOne's proprietary Level and Issuer pricing policies were expressed. Verifiable Claims are created based on the DID that the user owns by default, and are submitted when necessary, and are verified on the DID basis in the blockchain, thereby forming a trust relationship between interested parties.

OmniOne Token (OMN) enables exchange of value between an Issuer (which can verify a User's data and can issue a Verifiable Claim) and a Service Provider that seeks to provide a service needing identity/authentication by checking it via the blockchain without relying on an Identity Authority. The OMN token is used as the medium of exchange.

As DID-based Verifiable Claims are used, our ecosystem encourages OMN tokens to circulate to each Actor. We will show briefly how the OMN token is used in the demonstration.


5. Personal Information and OMNI Data Hub

DID has returned the sovereignty of personal identity information to individuals. With OmniOne, when personal information is submitted to be verified by an Issuer, that personal information can be used only for the purpose set by the User (its purpose and period for use) by using DID. This is unlike the centralized identity model, where personal information is stored and may used without the consent or knowledge of the user.

There has been a challenge to try to leverage the application of personal information in a decentralized way. For example, for a service which only needs identification or authentication from time to time, a decentralized system has not before been practical and a centralized system is an unnecessary burden from a security standpoint. With OmniOne's implementation of DID+FIDO, it is possible to securely store personal information in a distributed fashion, and to enable a high level of assurance for the identity information when it is used, and only when needed. In this way, not only is individual identity information unified, but personal information recovery and service accessibility becomes much easier when a device is lost or stolen.

OMNI Data Hub is provided for this purpose. Personal information is stored and distributed in the Data Hub safely at the individual's discretion and can be recovered at any time.

![img](https://lh3.googleusercontent.com/68VS5-vNLK4XF-_faQ2sy7y12S9KFTyMJ76cCNC4udUGb5sBWh-CCQcfMkSq3U36pUrHYdGOhxHqQFQP44LTqzPVrPyzV5FbRrjlfvyLKffleNtmWOP4j_uDQgDFxq6WW-aYug)
