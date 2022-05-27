Milestones with Parity:
 
## Milestone Number 1 [0-4 month]
 
Implementation of ciphertext-policy attribute-based encryption (CP-ABE) library according to the standard on ABE proposed in ETSI tech specification. 
Different from our Web 3.0 grant delivery, the library will be full-fledged, and guarantee the following functionalities: 
The CP-ABE library will be chosen-ciphertext secure and support decentralized and multi authorities and attribute revocation. 
We will provide full documentation on how to use the CP-ABE library in practice. 
The existing zero-pool pallet for data monetization will be modified according to the new CP-ABE scheme. Since our project will focus on access control in our future development, we will adapt the data monetization part of our project to the access control requirement.
 
### Milestone Number 2 [4-7 month]
 
1. Provide a setup mechanism for the decentralized authorities. 
2. Add an API for a Ruby token holder to become an authority. This includes a substrate pallet for the holder to stake Ruby token before officially becoming a verified authority. 
3. A specification for the authority on how to validate the user’s attributes. This specification will indicate how to translate standard access control policy into attribute universe, etc. 
4. A standard for converting an access-control policy into an attribute policy that can be used by the underlying encryption algorithms. Establish a secure and authenticated channel for the transfer of public parameters from the authority to the encryptor. An API for the encryptor to respond to the request for encryption. 
 
### Milestone 3 [7-10 month]
 
A standard for the attribute revocation mechanism. The standard will include the specification of the revocation list, and the time-based, and counter-based secret key revocation. 
An API for the encryptor to re-encrypt the ciphertext before revocation. An XCMP message layer for the notification mechanism between the encryptor and the event triggered by the update of the revocation list. 
A procedure for the authority to perform attribute revocation duty. This will include a backend algorithm for the authority to set up and maintain the attribute universe and attribute revocation list. It will also have an API for the authority to interact with the substrate pallet to update the revocation list.
Launch an access control service based on Substrate pallet. 
