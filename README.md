# Study of ID-based Ring Signatures and Implementation of Lattice-based Merkle Tree Accumulator

## 📄 Project Overview

* This report presents my Master’s Thesis Project, where I have explored the generic construction of an ID-based Ring Signature scheme.
* The primary focus of this work is the development of a lattice-based post-quantum Merkle Tree accumulator in C++.

## 🔒 Quantum Security

* A lattice-based hash function is used to ensure quantum security.
* The implemented accumulator takes n-dimensional vectors of identities (IDs)—which also serve as the public keys of the signature scheme—as input and accumulates the entire set (ring) of IDs, allowing for efficient storage and verification.

## ✅ User Validation

* A crucial feature of the system is the user validation process, where a user must prove that their ID belongs to the accumulated ring before signing a message.
* The signer first generates a witness for their corresponding ID, then generates a proof using the message, accumulated value, ID, and witness to verify the presence of their ID in the ring to the verifier.
* This proof itself acts as the signature on the message.

## 🛠️ Outcome

* The successful implementation of these components provides a foundation for further integration into a complete post-quantum ID-based ring signature system.

## 🔐 Applications

* Resistant to quantum attacks, this system can be used in:

  * Blockchain and cryptocurrencies
  * Secure messaging
  * Privacy-preserving authentication

