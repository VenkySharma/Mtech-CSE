### Lec1

### Lec2

### Lec3

### Lec4
Issue with perfect security in case of one time pad
- Malleability of one time pad.

  Given a ciphertext C1=E(K,P1), it should be impossible to create another ciphertext, C2, whose corresponding plaintext, P2, is related to P1 in a meaningful way (for example, to create a P2 that is equal to P1⊕1 or to P1⊕X for some known value X).

   Surprisingly, the one-time pad is malleable: given a ciphertext C1=P1⊕K, you can define C2=C1⊕1, which is a valid ciphertext of P2=P1⊕1 under the same key K.So if key is reused then this create a pattern of info from the ciphertext which is break to perfect security
- Length of the key(Unavodable)
  Because we don't want the key as long as our plaintext
