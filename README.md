These files contain calculations for the instantaneous stabilizer groups (ISGs) of our Floquet code examples. The Floquet codes can be identified by the folder name. 

Since the codes are translation invariant, we use polynomial representation. In this representation, we work out the circuits to map the ISGs to a canonical form. For example, for the 3D Floquet toric code ISGs, we construct circuits to map each ISG to copies of cubic lattice 3D toric code, and for the Floquet color code, we write circuits to map each ISG to two copies of toric code. 

We use the rewinding schedule GBRBGR for the 3D Floquet toric code. In both the G-rounds, the ISG is exactly the cubic lattice up to concatenation with 2-qubit repetition codes, thus no circuit is required. For a consistency check, we added the calculation for the number of logical qubits. For the B-rounds, we write the circuit to map the ISG to two copies of 3D toric codes and calculate the number of logical qubits. Due to the three non-local stabilizers (not included explicitly in the Mathematica files), we get 3 logical qubits instead of 6 for the two copies of 3D toric codes. For the R-round that immediately follows B, the ISG is equivalent to the one in B-round up to a basis change. The remaining ISG is the second R-round that immediately follows the G-round. For this one, we again get two copies of the 3D toric code as the ISG. However, the ISG generators include certain 3-qubit operators. 

For the 3D Floquet fermionic toric code, we write the circuits to map the ISG of the first round to a canonical form of the 3D fermionic toric code. The other ISGs are related by the symmetry of the 3D trivalent lattice on which we define the code. 

For the Floquet color code, we write the circuits to map the ISGs of two of the rounds since the other rounds are related to these two by symmetry. We also include the circuit for a parent stabilizer code which is equivalent to four copies of toric code; this is for a possible condensation picture of the Floquet color code. 


