# How The Mnemonic Phrase Works
>Basics you need to know  
>  
>1. What a “hash function” is  
>  
>2. What the SHA-256 hash algorithm is  
>  
>3. How a private key controls your account

# What is a hash? 

   A hash is equal to the sum of every number in an input. For example; in the input “1 2 3 4.” The hash would be 10. You get that hash by adding 1+2+3+4=10. The output “10” is like a summary of the input.  

   For the input “2 4 6 8 10” the hash output would be 2+4+6+8+10 = 30. So the hash of input “2, 4, 6, 8, 10” would be 30. 

   One special feature to note is that hashing is a “one-way function.” Meaning that if I just gave you the output of 30 there are actually many combinations of inputs that could result in the number 30.. 46,376 different possible combinations in the equation x+x+x+x+x=30

# What is the SHA-256 hash algorithm?

   Just like the equation above the SHA-256 algorithm is a hashing algorithm; albeit one that is much more complex. 

https://preview.redd.it/quwjprdck6v91.png?width=718&format=png&auto=webp&v=enabled&s=fea424786bea2a20742414e8585114d74a8e3b46

The input of the sha256 algorithm could be any amount of numbers, letters, or words and the output will always be a unique 256bit digit.

&#x200B;

https://preview.redd.it/31jnhkvgk6v91.png?width=703&format=png&auto=webp&v=enabled&s=d235c63d895eb3a8b134cdbf099ac9b84a47edad

Give it a shot for yourself using this link, [https://emn178.github.io/online-tools/sha256.html](https://emn178.github.io/online-tools/sha256.html) 

**Two important things to note:**  
   First, if you change any detail of the input, the entire output will be 100% completely unique, regardless of how small of a change you make. 

   Second, the input will always reproduce the same output. As long as the input is exactly the same as before, the output will also be the same. 

# Private keys and your wallet account

   Now that we’ve gone over some of the basics of hash functions and touched on the sha256 algorithm we can discuss how this ties into wallet security and what you need to know to protect your crypto. 

The 12/24 word mnemonic phrase *is* your wallet. When you use your 12/24 word mnemonic phrase as the input of the hashing algorithm the output of that algorithm *is* your private key. And that private key can be thought of as a 256bit long password to your wallet account on chain. 

https://preview.redd.it/rn3mw9jqn6v91.png?width=722&format=png&auto=webp&v=enabled&s=47aa14f0160582d47e5096a93d386487837735e4

Whenever you make a transaction, the chain verifies that you have the password or the “key” to authorize a transaction on the wallet account. 

This is why it is absolutely essential never to give anyone your mnemonic phrase. It’s not just a recovery phrase, it *is* your wallet. In decentralized finance, not even support or the project founders ever need to have your wallet. That is for you and you alone to have.

# Signing transactions and public key verification

   Having gone over how the private key string is produced we can go further over an example on how your public key is generated using your private key and how this is used to verify that only your private key is the key making tx.

   Same as using the mnemonic to generate a private key, the private key is also used in another algorithm to generate the public key. This algorithm is called elliptic curve cryptography or public key/private key cryptography

https://preview.redd.it/7w9s96y0o6v91.png?width=1180&format=png&auto=webp&v=enabled&s=74a6cd930bcb6229bbc48467767a051e610630ff

   This is how your public key is tied directly to your private key, because your public address is created by using the private key. 

   I'll have to come back to this and write more material on how using elliptic curve cryptography only your public key can be used to decrypt a signature made by your private key that is than verifiable for the blockchain to be used to submit the transaction to the chain

https://preview.redd.it/oag6jq58p6v91.png?width=1160&format=png&auto=webp&v=enabled&s=ac38d9236b0050a354812a5b65a813550d45e1f8

   But for now the main purpose of writing this is for everyone to better understand the importance of keeping your mnemonic phrase safe. It's not just a backup code or a recovery phrase, it is very much your private key. If you give this out to anyone or upload to websites you don't trust/verify, you are giving away your wallet to the person on the receiving end of that. 

   The foundation or dev team of any project has no database where your mnemonics are stored. We never need your mnemonic for any reason. This 12/24 word phrase is for you and you only. It is your sovereign control over your own financial accounts and what makes cryptocurrency so special. 

   If anyone is every asking you to input this mnemonic into anything for any reason be very skeptical. Know that on the other side of inputing that phrase is the output of your wallet account.