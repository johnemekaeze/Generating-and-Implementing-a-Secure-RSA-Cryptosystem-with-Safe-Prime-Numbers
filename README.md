# Generating and Implementing a Secure RSA Cryptosystem with Safe Prime Numbers

## Overview

This project demonstrates a secure RSA cryptosystem built using safe prime numbers. It covers the generation of two large safe primes (each with 600 digits), the creation of RSA keys (public and private), and the implementation of RSA encryption and decryption routines. Safe primes enhance security by ensuring both the prime $p$ and $\frac{p-1}{2}$ are prime.

## Key Features

- **Safe Prime Generation:**  
  Generates safe primes with exactly the specified number of digits, ensuring $p$ and $q$ are safe primes.

- **RSA Key Generation:**  
  Computes the RSA modulus $n = p \times q$, calculates Euler's totient $\phi(n) = (p-1)(q-1)$, selects a public exponent $e$ (typically 65537), and derives the private key $d$ as the modular inverse of $e$ modulo $\phi(n)$.

- **Encryption and Decryption:**  
  Implements RSA encryption (using $c = m^e \mod n$) and decryption (using $m = c^d \mod n$) to securely encode and decode messages.
