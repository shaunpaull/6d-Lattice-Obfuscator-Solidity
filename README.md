# 6d-Lattice-Obfuscator-Solidity
The LatticeEncryption contract implements a 6-dimensional lattice-based encryption scheme. It generates a large lattice with random symbols and complexities, connects the lattice nodes based on their positions, and provides functions to encrypt and decrypt messages using lattice indices.

It defines two struct types: LatticeSymbol represents a symbol in the lattice, and DAGNode represents a node in the lattice with its parents and associated symbol.
The contract constructor takes in parameters width, height, depth, time, energy, and spirit to determine the dimensions of the 6-dimensional lattice.
Upon contract deployment, the createLattice function generates random symbols and complexities for each lattice node.
The connectLatticeNodes function establishes connections (parent-child relationships) between lattice nodes based on their positions in the lattice.
The encryptMessage function takes a string message as input and converts it into an array of lattice indices by mapping each character to a lattice index.
The decryptMessage function takes an array of lattice indices and converts it back to a string by retrieving the corresponding characters based on the lattice indices.
The lattice is stored in the lattice mapping, where each lattice index is mapped to its corresponding DAGNode struct.
Overall, this contract provides a framework for creating and manipulating a 6-dimensional lattice, as well as encrypting and decrypting messages using the lattice indices.
