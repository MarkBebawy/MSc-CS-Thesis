A thesis submitted in fulfillment of the requirements for
the joint UvA-VU (University of Amsterdam & Vrije Universiteit) Master of Science degree in Computer Science.

# Title
Cryptographic Compilers for Linear Probabilistically Checkable Proofs

# Abstract
Probabilistically checkable proofs (PCPs) are proof systems in which the verifier
has restricted access to the prover’s proof. Their constructions are often
highly technical. By allowing for linear queries in the PCP model, resulting
in _linear probabilistically checkable proofs (LPCPs)_, the PCP constructions can
significantly be simplified. For LPCPs to be useful, cryptographic compilers are
needed that remove the idealized assumption of linear oracles by transforming
an LPCP into an interactive cryptographic protocol.
Currently, the best cryptographic compiler for LPCPs is based on _linear-
only encryption schemes_, which is heavy cryptographic machinery of which
the existence, although believable, does not rely on standard cryptographic
assumptions. The main goal of this thesis is to develop new cryptographic
compilers for LPCPs that rely on standard cryptographic assumptions. We developed
two such compilers that rely on the discrete logarithm assumption. Our
first compiler uses a _compressed Σ-protocol_ to realize the linear queries in an
LPCP. When compiling the _Hadamard LPCP_ for NP-relations with this compiler,
we get a cryptographic proof with logarithmic communication complexity,
and with the same asymptotic soundness error as the best current compiler.
Our second compiler is mostly useful for LPCPs that can cleverly be transformed
into _quadratic PCPs_ (which are LPCPs with quadratic queries instead
of linear queries) that have shorter proofs and fewer queries. We apply such
a transformation to the Hadamard LPCP, resulting in the _Hadamard QPCP_,
which combined with our second compiler results in a cryptographic proof with
roughly one third of the communication costs of our compiled Hadamard LPCP.
In summary, our new cryptographic compilers for LPCPs allow us to reap
the fruits of LPCPs, while still relying on standard cryptographic assumptions.
Furthermore, this thesis highlights the value of separating the information-
theoretic proof system from its cryptographic compiler to study these components in a modular fashion.

# Full thesis
[Download PDF](https://github.com/MarkBebawy/MSc-CS-Thesis/blob/main/MSc_CS_Thesis.pdf)

# Related literature study
[A Taxonomy of Probabilistic Proof Systems](https://github.com/MarkBebawy/MSc-CS-Thesis/blob/main/TaxonomyProofSystems.pdf)
