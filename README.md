# Low_light
📄 Low Light Enhancement & Secure Certificate Verification in MANETs
✨ Overview
This project presents a dual-focused contribution:

A deep learning-based approach for low-light image enhancement using an advanced U-Net architecture.

A secure certificate verification system for MANETs (Mobile Ad-hoc Networks) using threshold cryptography and BLS signatures.

🔍 Part 1: Low-Light Image Enhancement
🧠 Key Concepts
Based on Retinex theory to decompose images into reflectance and illumination.

Enhanced U-Net with:

Residual connections

Attention modules

Multi-scale fusion

Input: 4-channel image (RGB + max intensity)

Techniques: Spectral Normalization, Adversarial Training (GAN), and diverse loss functions

🛠️ Frameworks
PyTorch

Kornia

📈 Results
Improved image brightness and structure

Outperformed existing methods on SSIM and PSNR

🔐 Part 2: Secure Node Authentication in MANETs
🚨 Problem
MANETs are vulnerable to:

Passive/Active attacks

Lack of centralized infrastructure for PKI

🧩 Proposed Solution
A distributed PKI system using:

Shamir’s Secret Sharing with bivariate polynomials

Threshold Cryptography

BLS (Boneh-Lynn-Shacham) Signatures

🔧 Cryptographic Setup
Distributed key generation

Each node holds a partial secret

Nodes collaborate to:

Generate RSA keys

Sign & verify certificates

Certificates linked to node ID + public key

✅ Key Features
Certificate verification via bilinear pairing

Lightweight and efficient for resource-constrained nodes

Supports dynamic node join via interpolation

🧪 Example Use Case
Simulated with 4 nodes using elliptic curve over GF(4019)

Nodes define symmetric bivariate polynomials to share secrets

Node 5 joins by requesting shares from ≥3 existing nodes

Secure messaging achieved through public key encryption

📚 Technologies Used

Area	Tools / Concepts
Image Enhancement	PyTorch, Kornia, U-Net, GAN, Retinex Theory
Cryptography	Shamir Secret Sharing, RSA, BLS Signature
MANET Security	Threshold Cryptography, Bilinear Pairing
Mathematics	Polynomial Interpolation, Lagrange Coefficients
