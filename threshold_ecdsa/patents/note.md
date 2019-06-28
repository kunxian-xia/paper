# Note on Lindell's patent on 2-party ECDSA

Fig 1A and 1B is the *keygen* protocol. This corresponds to Protocol 3.1 in [Lindell's paper](https://eprint.iacr.org/2017/552).

In more detail, 
- Fig 1A describes the split of private key $x = x_1 * x_2$ as $(x_1, x_2)$.  

- Fig 1B describes how to pass $Enc(x_1)$ from party 1 to party 2. 


Fig 2 is the *2-of-2 sign* protocol. This corresponds to Protocol 3.2 in [Lindell's paper](https://eprint.iacr.org/2017/552).


## Implementation of Lindell17's scheme

1. Conner Fromknecht, [2pecdsa](https://github.com/cfromknecht/tpec), in *Golang*

2. Unbound-Tech, private repo, in C/C++ using libcrypto of *OpenSSL*

3. KZen-Network, [multi-party-ecdsa](https://github.com/KZen-networks/multi-party-ecdsa), in *Rust*.