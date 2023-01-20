# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: Web APIs & NLP

## Process

1. Call  reddit api via pushshift
2. Parse / clean data
3. Lemmatize / tokenize data
4. EDA, identify stopwords
5. Run models, tune hyperparameters
6. Review classification performance
7. All model comparison and review

## Description

**Problem Statement**

- How can we semantically identify the difference between /r/bitcoin and /r/ethereum, filtering for obvious terms? Many casual observers may these two assets together under the umbrella of 'crpytocurrency,' but the culture, evolution, design, and application of these blockchains are different, and have diverged substantially since 2015. Is it evident in posts on the respective subreddits?

- Enriching network (dao, token) data with user behavior and metadata is a rapidly growing market. We run an initial test on imbalanced classes (83% / 17%) to correctly predict the minority class. 


A brief history:

Bitcoin was initially launched as a decentralized monetary-policy based token, with the opportunity to act as a "decentralized computer" to transact value itself, or data lying within the the bitcoin blockchain (OP-return). Users quickly became excited about sending an arbitrarily small transaction, with data embedded in OP-return, using bitcoin as a carriage for any referenced dataset stored in OP-return.

Meanwhile, as bitcoin grew in popularity, demand for blockspace began to exceed blockspace supply - blocks became full. In general, any blockchain ecosystem trends toward (but not to) full blocks as arbitrary transactions are affordable until competition for space drives up fee pressure. 

The original whitepaper hardcoded the blocksize as a temporary measure, on which satoshi himself commented:

> It can be phased in, like: if (blocknumber > 115000) maxblocksize = largerlimit It can start being in versions way ahead, so by the time it reaches that block number and goes into effect, the older versions that don’t have it are already obsolete. (https://satoshi.nakamotoinstitute.org/posts/bitcointalk/485/)

At the time, jeff garzik, gavin andresen, and mike hearn were the primary core maintainers, variously had contact with satoshi, and were in favor of conservative growth. but several developers had become prominent contributors - Greg maxwell, peter todd, adam back, and luke dash jr. I encourage any reader to google these latter names - for they are various flavors of psychopaths, except for peter todd, who is just annoying. 

These latter contributors organized themselves behind a VC and private investment to create a startup called "blockstream," the only apparent value prop of which was that it was composed of several key core devs. 

Meanwhile, all bitcoin forums (reddit, bitcointalk, and the bitcoin wiki) were all maintained by a still unknown user named /u/cobra, who is either a sockpuppet account of greg maxwell, or simply sympathetic to their cause, or otherwise motivated.

What emerged was a manufactured constitutional crisis for bitcoin. The blockstream devs appeared to try to monetize their startup by strangling blockspace on Bitcoin, in order to force traffic onto their second layer network, lightning. They also degraded the network with segregated witness to make their lightning product possible, while invalidating the possibility of zero-confirmation transazations. Segwit was sold as a blocksize increase, while it was nothing of the sort - it segregated witness data and then subsidized the cost of these segwit blocks to make them appear larger. 

The blockstream devs pushed out the core devs, and social media was a key instrument in this exercise. Cobra-bitcoin owned (moderated) every major platform for bitcoin users, including reddit. Debate reached theological levels from the blockstreamers, and any "dissenting opinion" counter to the official blockstream platform was banned in cooperation with cobra bitcoin. 

At this point, all the banned and disgusted users left /r/bitcoin to its ivory tower, and started /r/btc. The bigger trend was the shift to ethereum. As bitcoin would never scale, nor adopt smart contracts or turing complete language, ethereum was now the only option. This is the great irony to the blockstream plan to strangle bitcoin traffic for their second layer - traffic simply went around the blockage onto other chains, primarily ethereum. This was a major moment in the growth of eth, as bitcoin essentially shut down in 2017 and now exists as something like a fixed income asset. 

To this day, ~1.5% of all BTC are held and transacted on the ethereum network, and WBTC is almost 40x larger than lightning (~$4B vs. $100m).

At this point, most people don't even know the history, as most users adopted after this constitutional crisis, which took place primarily on reddit. Can we spot the different users?





