Project Overview 
The goal of this project is to demonstrate that even mathematically strong cryptographic algorithms can be vulnerable due to implementation flaws. We focused on two critical attack vectors:
    1. Nonce Reuse Attack: Recovering the private key when the same random value ($k$) is used for different signatures.
    2. Timing Attack (Side-Channel): Extracting the secret key by analyzing the time variations during scalar multiplication.
Technologies 
    • Python 3.x — core logic and simulation scripts.
    • SageMath — advanced mathematical computations on elliptic curves.
    • Matplotlib/NumPy — statistical data analysis and visualization (CPA/SPA).
Key Results
    • Key Recovery: Successfully simulated a Timing Attack that recovers the secret key bits with 100% accuracy on unprotected implementations.
    • Statistical Proof: Developed correlation plots (Pearson correlation) that clearly visualize the leakages during bit-by-bit key processing.
    • Defense Implementation: Implemented and verified constant-time algorithms and RFC 6979 (deterministic nonce generation) which reduced attack success to a random guess level.
Authors
    • Yuliy Ostashkov
    • Lise Makarenko
