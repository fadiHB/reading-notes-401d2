# Introduction to Cryptography

Cryptography, or the art and science of encrypting sensitive information, was once exclusive to the realms of government, academia, and the military. However, with recent technological advancements, cryptography has begun to permeate all facets of everyday life.

Everything from your smartphone to your banking relies heavily on cryptography to keep your information safe and your livelihood secure.

And unfortunately, due to the inherent complexities of cryptography, many people assume that this is a topic better left to black hat hackers, multi-billion dollar conglomerates, and the NSA.

But nothing could be further from the truth.

## Understanding Ciphers: The Basis of All Cryptography

Cryptography, at its most fundamental level, requires two steps: encryption and decryption. The encryption process uses a cipher in order to encrypt plaintext and turn it into ciphertext. Decryption, on the other hand, applies that same cipher to turn the ciphertext back into plaintext.

Here’s an example of how this works.

Let’s say that you wanted to encrypt a the simple message, “Hello”.

So our plaintext (message) is “Hello”.

We can now apply one of the simplest forms of encryption known as “Caesar’s Cipher” (also known as a shift cipher) to the message.

With this cipher, we simply shift each letter a set number of spaces up or down the alphabet. 

So for example, the image below shows a shift of 3 letters.

Shift of 3 lettersMeaning that:

![img](https://cdn.shortpixel.ai/spai/w_671+q_lossy+ret_img+to_webp/https://thebestvpn.com/wp-content/uploads/2017/06/tFnX1co.jpg)

A = D
B = E
C = F
D = G
E = H
F = I
And so on.
By applying this cipher, our plaintext “Hello” turns into the ciphertext “Khoor”

To the untrained eye “Khoor” looks nothing like “Hello”. However, with knowledge of Caesar’s cipher, even the most novice cryptographer could quickly decrypt the message and uncover its contents.

## A Brief Word on Polymorphism

Before we continue, I want to touch on a more advanced topic known as polymorphism.

While the intricacies of this topic stretch far beyond the realm of this guide, its increasing prevalence mandates that I include a brief explanation.

Polymorphism is basically a cipher that changes itself with each use. Meaning that each time it is used, it produces a different set of results. So, if you encrypted the exact same set of data twice, each new encryption would be different from the previous one.

Let’s go back to our original example with the plaintext “Hello.” While the first encryption would result in “Khoor”, with the application of a polymorphic cipher, the second encryption could result in something like “Gdkkn” (where each letter is shifted down a rung of the alphabet)

Polymorphism is most commonly used in cipher algorithms to encrypt computers, software, and cloud-based information.

## Why Does Cryptography Matter?

I want to preface the rest of this article with a warning.

Throughout the rest of this article, I will be explaining exactly how cryptography works and how it is applied today. In doing so, I will have to employ a significant amount of technical jargon that may feel tedious at times.

But bear with me and pay attention. Understanding how all of the pieces fit together will ensure that you are able to maximize your personal security and keep your information out of the wrong hands.  

So before I go full blast, explaining symmetric and asymmetric cryptography, AES, and MD5, I want to explain, in Layman’s terms, why this matters and why you should care.

For starters, let’s discuss the only real alternative to cryptography, obfuscation. Obfuscation is defined as “The act of making something unclear, obscure, or unintelligible”. It means that, in order to transmit a secure message, you must hold back some of the information required to understand the message.

Which, by default, means it would only take one person with knowledge of the original message to divulge the missing pieces to the public.

With cryptography, a specific key and numerous calculations are required. Even if someone knew the encryption method used, they wouldn’t be able to decrypt the message without the corresponding key, making your information much more secure.

To understand why cryptography really matters you need look no further than something we all know and love, the Internet.

By design, the Internet was created to relay messages from one person to another, in a similar manner to the postal service. The Internet delivers “packets” from the sender to the recipient, and without the various forms of cryptography that we will discuss in a moment, anything that you sent would be visible to the general populace.

Those private messages you meant to send to your spouse? The whole world could see them. Your banking information?

Anybody with a router could intercept your funds and redirect them to their own account. Your work emails discussing sensitive company secrets? You might as well package those up and ship them to your competitors.

Luckily, we do have cryptographic algorithms that actively protect almost all of our personal data.

However, this does not mean that you are completely secure.

You need to look no further than recent attacks on companies like AdultFriendFinder and Anthem Inc. to realize that large corporations do not always implement the necessary systems required to protect your information.

Your personal security is your responsibility, no one else’s.

And the sooner that you can develop a strong understanding of the systems in place, the sooner you will be able to make informed decisions about how you can protect your data.  

## Types of Cryptography

* hashing
* symmetric cryptography
* asymmetric cryptography
* key exchange algorithms.

## The 4 Types of Cryptographic Functions

* Authentication
* Nonrepudiation
* Confidentiality
* Integrity

***done ..***