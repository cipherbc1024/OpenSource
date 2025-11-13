

### mpc core tss algorithms 

| protocols                              | usage                 | algorithms                                                                                                                            | remark | code reference |
|----------------------------------------|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------| ------ | ------------- |
| cmp20/cggmp21 threshold key generation | m out of n keygen     | ecdsa key geneation <br/> eddsa key generation<br/> hash commitment <br/> schnorr zk proof<br/>                                       |  N/A  |  tsslib |
| cmp20/cggmp21 threshold sign           | m out of n sign       | ecdsa /eddsa sign <br/>    Paillier Encryption <br/> Enc Range zk proof  <br/> Paillier affine group zk proof   <br/>                 |  N/A  |  tsslib  |
| frost eddsa threshold sign             | m out of n eddsa sign | eddsa sign                                                                                                                            |  N/A  |   tsslib  |
| cmp20/cggmp21  auxiliary               | auxiliary             | Paillier Encryption <br/>  Ring Pederson zk proof       <br/>  Paillier Blum    Modules zk proof <br/> No samll Factor zk proof <br/> |  N/A  |  tsslib       |


## mpc crypto table


| algorithm     | usage                                                                                              | remark   | code reference         |
|---------------|----------------------------------------------------------------------------------------------------|--------- |------------------------|
| ECIES Encrypt | Private Key Share Encryption <br/> User key backup                                                 | use KMS  | local ; go-etheruem ;github.com/ecies/go/v2   |
| AES  (GCM/CBC)         | For Communication Security; Hardware wallet to server ; mpc node to server ; encrypt transaction ; | generate random key for every session       | local / golang std lib |
| SHA256 /SHA3       | Common  Hashing                                                                                    | N/A     | local / golang std lib |
| pbkdf2       | Password based key derivation  for Bip39                                                           | N/A     | local / golang std lib |
| HMAC-SHA512  | Bip32 key derivation                                                                             | N/A     | local / golang std lib |
| Google Auth  | Running Server in Production                                                                       | N/A     | |
|  ECDH        | For key agreement ; node to server communication                                                   | N/A     | local / golang std lib |
|  Ed25519  Signature    | For node to server communication authentication                                                    | N/A     | local / golang std lib |
|  RSA Signature    | sign wallet address ; sign request to HBC Business                                                 | N/A     | local / golang std lib |
| RSA Encryption | Encrypt wallet backup key; Server TLS Certification                                                | N/A     | local / golang std lib |
|  JWT with AES encryption       | For user  to server communication authentication                                                   | N/A     | local / golang std lib |
|  KMS        | store private key share                                                                            |  Aliyun KMS     |  |



