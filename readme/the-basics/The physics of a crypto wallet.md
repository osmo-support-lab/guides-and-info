# The physics of a crypto wallet

Private keys, Public keys, Mnemonic Seed phrase, Cold Storage, Hot wallet...Maybe you've heard of these terms but what do they all mean? How are they all connected? The goal of this article is to give you a basic understanding of wallets, how they work, and most importantly how you can keep yourself secure

# Public key / Private key encryption (Asymmetric Encryption)

YouTube video to dive deeper into the science:[ https://www.youtube.com/watch?v=wXB-V\_Keiu8&t=3s](https://www.youtube.com/watch?v=wXB-V_Keiu8&t=3s)

**Public-key cryptography**, or **asymmetric cryptography**, is a cryptographic system that uses pairs of keys. Each pair consists of a *public key* (which may be known to others) and a *private key* (which may not be known by anyone except the owner). The key pairs are based on mathematical problems termed "one-way functions." Meaning that funds can be only sent to\* the public key or only sent from\* the private key. Effective security requires keeping the private key private; the public key can be openly distributed without compromising security.

# Mnemonic Seed Phrase

Your **seed phrase** is a mnemonic code consisting of 12-24 words that is used to recover your cryptocurrency wallet. Sometimes called a backup phrase, recovery phrase, or mnemonic sentence - it is the foundation of most modern wallets and the crypto universe in general. **Do not ever give out this phrase to anyone.**

Wallet software will typically generate a seed phrase and instruct the user to write it down on paper. If the user's computer breaks or their hard drive becomes corrupted, they can download the same wallet software again and use the paper backup to get their bitcoins back.

Anybody else who discovers the phrase can steal the bitcoins, so it must be kept safe like jewels or cash. For example, it must not be typed into any website or even given to people claiming to be support. Nobody ever needs to see this phrase.

Your Mnemonic seed **IS** your private key mentioned above. **So if you give someone this phrase, you are effectively giving them ownership over your wallet.** A simplified explanation of how seed phrases work is that the wallet software has a list of words taken from a specific dictionary --- The English-language wordlist for the BIP39 standard --- with each word assigned to a number. The seed phrase can be converted to a number which is used during the crafting of the key at specific mathematical intervals to arrive at the final point which is your private key. You can think of each word in your seed phrase like a groove in a key that allows you to unlock your specific wallet. [https://github.com/bitcoin/bips/blob/master/bip-0039/bip-0039-wordlists.md ](https://github.com/bitcoin/bips/blob/master/bip-0039/bip-0039-wordlists.md)<- This is the 2048 list of words used in the BIP39 standard

# How secure is the private key

Crypto wallets use a security hashing algorithm called SHA-256. In this algorithm you would take your 24 word seed phrase and run it through something called a "Merkle Tree" and you output a 256-bit string of 0's and 1's that is unique to your specific seed phrase. Every key in crypto is 256 bits long and the final hash (your public address) is 160 bits long. A brute-force attack on your private key would need to make 2^(256) attempts to generate the exact pattern of 0's and 1's that represent your key. To give you some insight into how big this number is, In order for a computer to guess each key after key in hopes of getting your key, it would take that computer 27 trillion trillion trillion trillion trillion years. The universe itself is 15 billion years old.

Another important detail. Having two private keys with the same hash value (called a collision) is extremely unlikely. With 2^(256) possible keys, you could have more key options than the number of atoms in the visible universe. 

&#x200B;

115,792,089,237,316,195,423,570,985,008,687,907,853,269,984,665,640,564,039,457,584,007,913,129,639,936 <- this is what the size of 256 numbers look like. And someone would have a 1 in that many chances of accurately guessing your key.

&#x200B;

The only flaw in this security would be if you were to give away your 24 mnemonic phrase