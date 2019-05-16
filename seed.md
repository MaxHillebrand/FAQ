FAQ regarding bitcoin seeds.
By [6102bitcoin](https://twitter.com/6102bitcoin)

# Index

1) [**The Basics**](#1-The-Basics)
	- [Introduction](#Introduction)
	- [Terminology](#Terminology)
	- [What is a HD Wallet?](#What-is-a-HD-Wallet)
2) [**Creating your seed**](#2-Creating-your-seed)
	- [Where should I physically be when I backup my seed?](#Where-should-I-physically-be-when-I-backup-my-seed)
	- [All seeds are not created equal](#All-seeds-are-not-created-equal)
	- [Does the order of the words matter?](#Does-the-order-of-the-words-matter)
	- [How do I get my seed?](#How-do-I-get-my-seed)
	- [Should I check my seed?](#Should-I-check-my-seed)
3) [**Storing your Seed**](#3-Storing-your-Seed)
	- [Why should I bother storing my seed, I only have a small amount of bitcoin?](#Why-should-I-bother-storing-my-seed-I-only-have-a-small-amount-of-bitcoin)
	- [Should I have multiple (redundant) backups?](#Should-I-have-multiple-redundant-backups)
	- [How can I store my seed](#How-can-I-store-my-seed)
	- [Can I 'encrypt' my seed so that all is not lost if someone finds my mnemonic?](#Can-I-encrypt-my-seed-so-that-all-is-not-lost-if-someone-finds-my-mnemonic)
	- [Paper Backups](#Paper-Backups)
	- [Metal Backups](#Metal-Backups)
	- [Should I split my mnemonic in two and Hide 6 words in Location A & 6 words in Location B?](#Should-I-split-my-mnemonic-in-two-and-Hide-6-words-in-Location-A-&-6-words-in-Location-B)
4) [**Using your Seed**](#4-Using-your-Seed)
	- [Can I recover my bitcoin without my seed?](#Can-I-recover-my-bitcoin-without-my-seed)
	- [How should I recover bitcoin using my seed?](#How-should-I-recover-bitcoin-using-my-seed)
	- [What is the Derivation Path?](#What-is-the-Derivation-Path)
	- [How often should I check backups?](#How-often-should-I-check-backups?)

# 1) The Basics

### Introduction

Great - you have decided to control your bitcoin directly instead of using a custodial service like an exchange. This is a very wise move - exchanges fall into only two categories; those which have already been hacked and those which will be hacked in #twoweeks.

By holding your own keys, you (and only you) are able to spend your bitcoin. You should take time to read this FAQ in order to understand the common errors & mistakes, and to learn the best practice in seed management. 

### Terminology

When it comes to bitcoin seed descriptions, words are often confused and used interchangeably. It is important that we speak a common language, so let me define what I mean by each of these words.

| Word | Definition | Other Names |
| ---- | ---- | ---- |
| [**Private key**](https://en.bitcoin.it/wiki/Private_key) | A secret 256 bit number you use to spend bitcoin| secret key | 
| [**Mnemonic**](https://en.bitcoin.it/wiki/Seed_phrase) | A list of words in a specific order which can be used to generate a bitcoin private key | seed phrase / seed words |
| [**Seed**](https://bitcoin.org/en/glossary/hd-wallet-seed) | A potentially short value that is used to generted the master private key. | seed / secret |
| **Non-Extended Mnemonic** | 12/24 Words (Just the Mnemonic) | Seed Words | 
| **Extended Mnemonic** | 13/25 Words: Mnemonic (12/24 words) + Passphrase (1 word)) | | 
| **Backup** | A complete set of information from which your bitcoin can be recovered (i.e. your seed, master private key, used derivation paths)  | |
| **Encrypted Backup** | Backup encrypted with a password (not to be confused with a passphrase) | |

### What is a HD Wallet?

In practice, most bitcoin wallets are 'HD' (Hierarchical Deterministic) wallets - This means that a single bitcoin private key is used to generate as many key pairs as is required. This makes it easy for the user to use a new address each time they receive bitcoin, which is how bitcoin is designed to be used. 

With a HD wallet the bitcoin private key (which is determined using your seed) is combined with something called a 'chain code' to generate what is referred  to as a 'master extended key'.

Your bitcoin seed is all the information required to recover your bitcoin private keys. Typically this is presented to you by your wallet as a mnemonic - a series of either 12 or 24 words from [this list](https://github.com/bitcoin/bips/blob/master/bip-0039/english.txt) which can be used to generate your private keys following [BIP39](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki#). 

Many wallets will simply present you the mnemonic calling it your 'private keys' your 'seed words'. 

All seeds generated using BIP39 actually consist of the mnemonic + a passphrase.

More secure wallets will give you the option to set a passphrase (not to be confused with a password). 

Anyone with access to your seed and passphrase can spend your coins. 
As such it is imperative that you store copies of your seed securely. 

# 2) Creating your Seed

### Where should I physically be when I backup my seed?

Remember that if anyone sees your seed it is potentially compromised, and should be treated as such. 
For this reason make sure that you backup your seed somewhere that is private and that has no cameras/CCTV. 
- Don't read your seed aloud as someone could hear it. 
- Don't type it into a computer
- Don't take a picture / screenshot

### All seeds are not created equal

Suppose you have a computer riddled with malware and viruses and you download some bitcoin wallet software and view the mnemonic. This mnemonic is likely insecure. The viruses/malware may be taking screenshots of your computer at regular intervals and sending this data to the creator of the virus/malware. 
If you can see your seed on screen, then potentially so can the hacker.

For this reason, when non-trivial amounts of bitcoin it is crucial that you carefully control the environment in which the seed is generated. The easiest way for non-technical people to do this is to buy a 'Hardware Wallet'. These devices store all the 'secret information' required to access your bitcoin on the dedicated hardware device so that it doesn't matter if your computer has viruses/malware. 

That said, some hardware wallets are better than others so make sure that you never enter your seed into your computer - only enter it into the device itself.

### Does the order of the words matter?
Yes! The order of the words does matter. You must store your seed in such a way that the order of the words is clear and unambiguous. 

### How do I get my mnemonic?

This will depend on the bitcoin wallet that you are using. Most have a 'backup seed' option visible in the settings menu which can be used at any time, though some only allow seed backups when the wallet is initialised. 

It is important to note that it is generally insecure to create your own seed (i.e. a [Brain Wallet](https://en.bitcoin.it/wiki/Brainwallet)). 

### Should I check my mnemonic?

You should definitely check your backup as part of your process for backing up. Failure to do so could lead to you losing your bitcoin - don't risk it.

# 3) Storing your Mnemonic

### Why should I bother storing my mnemonic, I only have a small amount of bitcoin.

The value of bitcoin could increase substantially and you may one day regret not backing up your seed. You should **always** back up your seed with a mnemonic. It is good practice to regularly review your seed management and consider how effective your chosen solution is.

### Should I have multiple (redundant) backups of my seed?

Yes. For the reasons explained below you should have multiple redundant backups of your seed.

### How can I store my seed?
Initially let us consider the case where you store a single unencrypted mnemonic (12 or 24 words). 

| Method  						   	|----          				| Digital Theft Resistance 	| Physical Theft Resistance 		| Durability 						|
| ------    					    | ---- 				    		| -------------------------	| ------------------------------|	---------------				|
| Screenshot              | On Phone 					  | Weak							        | Weak													|	Fragile (Deletion) 		|
| Notes App               | On Phone					  | Weak							        | Weak													|	Fragile (Deletion)		|
| Printed Paper Note  		| In Home 					  | Weak							        | Weak													|	Fragile (Fire)	  		|
| Printed Paper Note 			| Bank Deposit Box 		| Weak							        | **Strong**										|	**Durable**        		|
| Handwritten Paper Note  | In Home 					  | **Strong**				        | Weak													|	Fragile (Fire)	  		|
| Handwritten Paper Note  | Bank Deposit Box 		| **Strong**				        | **Strong**										|	**Durable**        		|
| Handwritten Paper Note  | Buried Somewhere 		| **Strong**				        | **Strong**										|	Fragile (Water)				|
| Stamped Metal Sheet [1]	| In Home 					  | **Strong**				        | Weak													|	**Durable**        		|
| Stamped Medal Sheet	    | Bank Deposit Box 		| **Strong**				        | **Strong**										|	**Durable**        		|
| Stamped Medal Sheet	    | Buried Somewhere 		| **Strong**				        | **Strong**										|	**Durable**        		|
| USB (Plaintext)					| In Home 						| **Strong**				        | Weak													|	Fragile (Water/Time)	|
| Memorised	[2]						| Brain								| **Strong**				        | **Strong**										|	Fragile (Time/Injury)	|

*[1] There are many ways to do this, some are better than others - see Lopp's [initial comparison](https://medium.com/@lopp/metal-bitcoin-seed-storage-stress-test-21f47cf8e6f5) & [more recent comparison](https://youtu.be/zFN__b6ARH4?t=20593)*

*[2] Often referred  to as a [Brain Wallet](https://en.bitcoin.it/wiki/Brainwallet) - Not to be confused for a wallet which you generate the mnemonic using your brain (i.e. sentence from a book) a Brain Wallet is a wallet for which you have memorised a mnemonic which was generated securely using a source of entropy.*

There are three methods that are both durable and resistant to theft;
- Handwritten Paper Note in a Bank Deposit Box
- Stamped Metal Sheet in a Bank Deposit Box
- Stamped Metal Sheet Buried Somewhere

A Bank Deposit Box is fine, but it requires some degree of trust in the bank.
Burying is fine, but it requires some degree of luck that someone won't find it / that you will be able to find it.

In either case, theft of the seed can occur. Theft of an unencrypted seed is bad for two reasons;
A) The thief can spend your coins at any time. If they replace the seed there is no way for you to know that the seed is compromised. 
B) You have lost your backup. You are unable to restore your seed, thus your bitcoin is lost whether or not the thief sweeps the funds. 

You can use a watch only wallet to monitor the balance of your addresses, though if you see your funds move it is too late to do anything about it. Furthermore, if someone finds your watch only wallet they know how much bitcoin you have.

If you notice that your seed has been stolen you want to be able to quickly move your funds in-case the thief hasn't figured out what they stole, or they simply haven't swept the funds yet. For this reason is obvious that you should have MULTIPLE seed backups.

But with an **unencrypted seed**, each additional backup is an additional risk, because theft of any one of your backups is enough for a thief to steal your bitcoin. It would be better if you encrypted your seed, so that the thief wouldn't be able to steal your funds if they only have your 12/24 word mnemonic. 

### Can I 'encrypt' my seed so that all is not lost if someone finds my mnemonic?

Yes, you can encrypt your mnemonic by one of two methods:

#### 1) Use a passphrase alongside your mnemonic following [BIP39](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki#from-mnemonic-to-seed)

Behind the scenes, all wallets following BIP39 (pretty much all wallets) are actually using a passphrase of "" (an empty string). 
Some wallets will let you set a custom passphrase which combined with your mnemonic forms your seed.
	
Note, the passphrase is sometimes referred to as a "seed extension", "extension word" or "the 13th/25th word".

#### 2) Encrypt the plaintext seed words

You can take your mnemonic words and use any encryption method to ensure that you need to use a password to decrypt the file. 
You use either Physical or Digital Encryption Tools;

- **Physical Encryption Tool** ([e.g. Enigma](https://en.wikipedia.org/wiki/Enigma_machine) / [One Time Pad](https://en.wikipedia.org/wiki/One-time_pad)): Clearly if you are using a physical encryption tool you will need to ensure that the tool is commonly available so that you can decode when required. Enigma Machines are hard to come by - so they are not a practical solution. The One Time Pad provides perfect encryption, but remember - anyone with physical access to the pad can decode the mnemonic.
- **Digital Encryption Tool** ([e.g. VeraCrypt](https://www.veracrypt.fr/en/Home.html)): If you are using a digital encryption tool you will need to ensure that the computer on which you are encrypting/decrypting data is secure. The easiest way to do this is to use a temporary OS like [tails](https://tails.boum.org) on an old computer which is not connected to the internet. 
	
### Paper Backups

If you do decide to use a paper backup:
- Use waterproof ink & paper
- Write on a hard surface so you don't indent the paper below

Learn More: [Here](https://www.quora.com/How-do-I-maintain-a-paper-notebook-that-can-remain-for-years) and [Here](https://www.quora.com/If-I-write-with-a-pencil-on-my-notebook-will-the-writing-last-for-a-long-time-say-50-years-or-will-it-just-fade-away-gradually)

### Metal Backups

There are lots of options available. See Lopp's [initial comparison](https://medium.com/@lopp/metal-bitcoin-seed-storage-stress-test-21f47cf8e6f5) & [more recent comparison](https://youtu.be/zFN__b6ARH4?t=20593).
The [Blockplate 1.0](https://www.blockplate.com/) appears to hold up well to fire / crushing while being easy to use.

### Should I split my mnemonic in two and Hide 6 words in Location A & 6 words in Location B?

This reduces the cryptographic security of your backup (it is far easier to brute force the private key with 6 mnemonic words already known than with none known). 

That said, the thief would have to know what the 6 words are and either spend time cracking the seed themselves or sell the seed to someone who would have no way to know the bitcoin they could steal before cracking the seed (so may be unwilling to pay for the first/last 6 words). 

It is much better to use [Shamir's secret sharing](https://en.wikipedia.org/wiki/Shamir%27s_Secret_Sharing) to split the seed into 2 secrets, this way each piece of information is useless in isolation, and it is impossible to brute force the private key. The secrets can be recombined to recover the seed. You can also add redundancy, requiring say 2 of 3 of the secrets, or 3 of 5 (or any N of M). [Trezor](https://trezor.io) are very close to a release of their own implementation of Shamir's secret sharing, [SLIP 39](https://github.com/satoshilabs/slips/blob/master/slip-0039.md).

# 4) Using your seed

### Can I recover my bitcoin without my seed?
No. Typically it is not possible to recover your bitcoin unless you have your seed. **Lose your seed, Lose your bitcoin**.

### How should I recover bitcoin using my seed?

You should follow the same rules when recovering bitcoin using your seed as when you are generating your seed;
- Carefully control the environment in which the seed is exposed. The easiest way for non-technical people to do this is to buy a 'Hardware Wallet'. These devices store all the 'secret information' required to access your bitcoin on the dedicated hardware device so that it doesn't matter if your computer has viruses/malware. That said, some hardware wallets are better than others so make sure that you never enter your seed into your computer - only enter it into the device itself.

Remember that if anyone sees your seed it is potentially compromised, and should be treated as such. 
For this reason make sure that you recover bitcoin from your seed somewhere that is private and that has no cameras/CCTV. 
- Don't read your seed aloud as someone could hear it. 
- Don't type it into a computer

### What is the Derivation Path?

[StackExchange](https://bitcoin.stackexchange.com/questions/78993/default-derivation-paths)
	
### How often should I check backups?

You should definitely check your backup as part of your process for backing up. Provided that you have done this correctly there should be no need to actually sweep bitcoin from the backup unless you need the bitcoin. It is worth checking that the backup remains accessible at irregular intervals (say every 1-3 years). It is worth checking because if a single backup disappears you can recover using a secondary backup (if there is a chance that the backup was stolen) or make a replacement backup (if you are completely confident that the backup was just damaged, e.g. house fire). Don't regularly check backups (e.g. the 1st Jan each year) as this could be obvious and lead to people discovering your backup.
