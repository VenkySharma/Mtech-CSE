### [Lec1]() -

### [Lec2]()-*08/01/24*

### [Lec3]()-*10/01/24* 

### Lec4
Issue with perfect security in case of one time pad
- Malleability of one time pad.

  Given a ciphertext C1=E(K,P1), it should be impossible to create another ciphertext, C2, whose corresponding plaintext, P2, is related to P1 in a meaningful way (for example, to create a P2 that is equal to P1⊕1 or to P1⊕X for some known value X).

   Surprisingly, the one-time pad is malleable: given a ciphertext C1=P1⊕K, you can define C2=C1⊕1, which is a valid ciphertext of P2=P1⊕1 under the same key K.So if key is reused then this create a pattern of info from the ciphertext which is break to perfect security
- Length of the key(Unavoidable)

  Because we don't want the key as long as our plaintext
- Why Under the same key OTP was unsafe

  Because no matter what ever you do human is weak in generating randomness. This will be exploited under the same key.
  Human weakness in generating randomness e.g
  - Financial Data statistics
  - Password statistics

So, Now the solution remains under the umbrella that we will have to relax security requirement.
We dont want our solution to be perfectly secure. What are the security requirement or how we want our security to be defined?
There are two methods:
1. Concrete Security Level
2. Asymptotic Security Level

### [Lec5]()-*15/01/24*

### [Lec6]()-*17/01/24* 

### [Lec7]()-*22/01/24*

### [Lec8]()-*24/01/24* 

### [Lec9]()-*29/01/24*

### [Lec10]()-31/01/24* 

### [Lec11]()-*05/02/24*

### [Lec12]()-*07/02/24* 

### [Lec13]()-*12/02/24*

### [Lec14]()-*14/02/24* 

### [Lec15]()-*19/02/24*
GCD, Extended GCD, Chinese Remainder Theorem, Square Root Mod n, Test for Primality, Miller Rabin Test

### [Lec16]()-*26/02/24* 
Proof of Correctness of RSA, Attack on Rsa, Rabin Cryptosystem, Square Root mod n

### [Lec17]()-*28/02/24*
Test for Primality, Using CRT, charmicel number, Miller Rabin Test, Elgamal Cryptosystem

### [Lec18]()-*01/03/24*
Quadratic Residue Modulo p, QNR, Euler's criterion

### [Lec19]()-**

### [Lec20]()-** 

