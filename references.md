# TmMgGaO₄ Quantum Twin — References

Reference material for simulating the frustrated triangular-lattice antiferromagnet TmMgGaO₄ on a Rydberg atom array.

## The material

**[1]** Cevallos, Stolze, Kong & Cava, *Anisotropic magnetic properties of the triangular plane lattice material TmMgGaO₄*, Mater. Res. Bull. **105**, 154 (2018).
Discovery and synthesis. Crystal structure; Tm³⁺ on a triangular net.

**[2]** Shen et al., *Intertwined dipolar and multipolar order in the triangular-lattice magnet TmMgGaO₄*, Nat. Commun. **10**, 4530 (2019). [arXiv:1810.05054](https://arxiv.org/abs/1810.05054)
Neutron scattering. Three-sublattice order gives a magnetic Bragg peak at the **K point** — the order parameter the simulation must reproduce.

**[3]** Li et al., *Partial up-up-down order with the continuously distributed order parameter in the triangular antiferromagnet TmMgGaO₄*, Phys. Rev. X **10**, 011007 (2020).
Magnetisation data for comparison against emulation.

## The model

**[4]** Chen, *Intrinsic transverse field in frustrated quantum Ising magnets*, Phys. Rev. Research **1**, 033141 (2019).
Why a non-Kramers ion's two-singlet ground state acts as an intrinsic transverse field.

**[5]** Liu, Huang & Chen, *Intrinsic quantum Ising model on a triangular lattice magnet TmMgGaO₄*, Phys. Rev. Research **2**, 043013 (2020). [arXiv:1909.03608](https://arxiv.org/abs/1909.03608)
Establishes TmMgGaO₄ as the transverse-field Ising antiferromagnet on a triangular lattice. **The basis of the whole mapping.**

## Frustration and order by disorder

**[6]** Wannier, *Antiferromagnetism. The triangular Ising net*, Phys. Rev. **79**, 357 (1950). Erratum: Phys. Rev. B **7**, 5017 (1973).
Extensive ground-state degeneracy; residual entropy ≈ 0.323 k_B/site. The classical model never orders.

**[7]** Moessner & Sondhi, *Ising models of quantum frustration*, Phys. Rev. B **63**, 224401 (2001).

**[8]** Isakov & Moessner, *Interplay of quantum and thermal fluctuations in a frustrated magnet*, Phys. Rev. B **68**, 104409 (2003).
[7]+[8]: how a transverse field selects three-sublattice order via quantum order by disorder.

**[9]** Li et al., *Kosterlitz–Thouless melting of magnetic order in the triangular quantum Ising material TmMgGaO₄*, Nat. Commun. **11**, 1111 (2020).

**[10]** Hu et al., *Evidence of the Berezinskii–Kosterlitz–Thouless phase in a frustrated magnet*, Nat. Commun. **11**, 5631 (2020).
Experimental counterpart to [9].

**[11]** Dun et al., *Neutron scattering investigation of proposed Kosterlitz–Thouless transitions in the triangular-lattice Ising antiferromagnet TmMgGaO₄*, Phys. Rev. B **103**, 064424 (2021). [arXiv:2011.00541](https://arxiv.org/abs/2011.00541)
Inelastic neutron scattering fixes the effective Hamiltonian parameters. **Source for numerical values of J and Γ.**

## Rydberg platform

**[12]** Scholl et al., *Quantum simulation of 2D antiferromagnets with hundreds of Rydberg atoms*, Nature **595**, 233 (2021). [arXiv:2012.12268](https://arxiv.org/abs/2012.12268)
196 atoms; square **and** triangular arrays. The warm-up target.

**[13]** Leclerc et al. (PASQAL), *One-to-one quantum simulation of the low-dimensional frustrated quantum magnet TmMgGaO₄ with 256 qubits*, arXiv:2603.20372 (2026). [arXiv:2603.20372](https://arxiv.org/abs/2603.20372)
Closest existing work. 256-qubit Rydberg simulator of the TmMgGaO₄ Hamiltonian; magnetisation matches single-crystal susceptibility. Keeps both J₁ and J₂; probes the paramagnet → 1/3-order (√3×√3) transition; adds snapshot analysis and quench dynamics.

## Tools

- [Pulser](https://github.com/pasqal-io/Pulser) — pulse-level programming ([docs](https://pulser.readthedocs.io))
- emu-mps / emu-sv — tensor-network and state-vector emulators

## Reading order

[1] → [5] → [2] for the material and model. [6], [8] for the ordering mechanism. [11] for Hamiltonian parameters. [12] → [13] for the simulation protocol.
