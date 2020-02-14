---
layout: post
title:  "Thoughts on Bitcoin vs. quantum computing"
date:   2019-12-13 21:40:25 -0500
categories: blog
---
# Observations on Bitcoin network vs. quantum computing
&nbsp;

A common fear I hear throughout the spheres of crypto, Twitter, and independent investment is the question of Bitcoin's resilience, and more broadly, cryptographic resilience as a whole, in the face of quantum computers - will the Bitcoin network and your bank's security be rendered worthless and destroyed by scalable quantum tech? Let's think about it.
&nbsp;

Some background for the uninitiated: Bitcoin's inherent scarcity, the main thing that fuels its fundamental value, is a product of cryptography and computer science theory. Cryptography obscures (encrypts) data by relying on the fact that its hard for a computer to factor big numbers, but easy to multiply them. Encryption is applying mathematics in the public sphere to transform information into an unreadable form and to cut a key to decipher it. With that secret key, you restore the readable data. Though factoring numbers is not fast, it’s not impossible. With classical computers, it would take our most powerful machine longer than the existence of the known universe to break existing RSA encryption.
&nbsp;

Interjection: "military grade encryption." Have you heard this phrase? It's a meme, and a successful one at that. Your Facebook account is "as encrypted" as the military is.
&nbsp;

When quantum computers can scale, all commonly used public key algorithms will be broken. RSA, elliptic curve, and so on. On one hand, at present Bitcoin does have some resilience if using a wallet address a single time, but this method is basically a proxy for real security and could easily be tripped up by inattentiveness.
&nbsp;

We're more interested in __post-quantum cryptography__, *specifically*, in my case, that type of [post-quantum crypto developed by Chris Peikert][peikert-crypto], a former professor of mine at Michigan -- Go Blue.
&nbsp;

Dr. Peikert's public key crypto based on lattices and polynomial rings (over my head) will put your worries at ease and your tokens out of harm's way. It is bona fide designed to be secure against an adversary in possession of a powerful quantum computer.
&nbsp;

All that's required is a software modification to the Bitcoin source that swaps out crypto modules from antiquated to updated. Take the elliptic curve public key infrastructure and replace it with a PKI that relies on lattices/rings. Follow it up with a soft fork, and your BTC network just became quantum-cool.
&nbsp;

[peikert-crypto]: https://en.wikipedia.org/wiki/Ring_learning_with_errors_key_exchange
