# EX-NO-10-Diffie-Hellman-Key-Exchange-Algorithm

## AIM:
To Implement Diffie Hellman Key Exchange Algorithm 

## Algorithm:

1. Diffie-Hellman Key Exchange is used for securely sharing a secret key between two parties over an insecure channel.

2. Initialization: Agree on a large prime number \( p \) and a primitive root \( g \) modulo \( p \) (both are public values).

3. Key Exchange Process: 
   - Each party selects a private key and calculates their public key using the formula \( g^{\text{private key}} \mod p \).
   - Each party then shares their public key with the other.

4. Secret Key Computation: 
   - Each party computes the shared secret key using the received public key and their own private key.

5. Security: The difficulty of computing discrete logarithms ensures that the shared key remains secure even if public values are intercepted.

## Program:
```
# Diffie Hellman Key Exchange Algorithm in Python

# Public values
p = 23
g = 5

# Private keys
a = 6
b = 15

# Public keys
A = (g ** a) % p
B = (g ** b) % p

print("Public Key of A:", A)
print("Public Key of B:", B)

# Shared Secret Keys
key_A = (B ** a) % p
key_B = (A ** b) % p

print("Secret Key for A:", key_A)
print("Secret Key for B:", key_B)

```


## Output:

<img width="360" height="244" alt="image" src="https://github.com/user-attachments/assets/b223c802-4cfa-4527-90aa-5d31698da09e" />


## Result:
  The program is executed successfully

