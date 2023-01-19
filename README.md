# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: Web APIs & NLP

### Description

**Problem Statement**

- How can we semantically identify the difference between /r/bitcoin and /r/ethereum, filtering for obvious terms? Many casual observers may these two assets together under the umbrella of 'crpytocurrency,' but the culture, evolution, design, and application of these blockchains are different, and have diverged substantially since 2015. Is it evident in posts on the respective subreddits?

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


## Process

1. Call  reddit api via pushshift
2. Parse / clean data
3. Lemmatize / tokenize data
4. EDA, identify stopwords
5. Run models, tune hyperparameters
6. Review classification performance
7. All model comparison and review



---

### Necessary Deliverables / Submission

- Code must be in at least one clearly commented Jupyter Notebook.
- A readme/executive summary in markdown.
- You must submit your slide deck as a PDF.
- Materials must be submitted by **9:30 AM (ET) on Friday, Jan. 20th**.

---

## Rubric
Your instructors will evaluate your project (for the most part) using the following criteria.  You should make sure that you consider and/or follow most if not all of the considerations/recommendations outlined below **while** working through your project.

For Project 3 the evaluation categories are as follows:<br>
**The Data Science Process**
- Problem Statement
- Data Collection
- Data Cleaning & EDA
- Preprocessing & Modeling
- Evaluation and Conceptual Understanding
- Conclusion and Recommendations

**Organization and Professionalism**
- Organization
- Visualizations
- Python Syntax and Control Flow
- Presentation

**Scores will be out of 30 points based on the 10 categories in the rubric.** <br>
*3 points per section*<br>

| Score | Interpretation |
| --- | --- |
| **0** | *Project fails to meet the minimum requirements for this item.* |
| **1** | *Project meets the minimum requirements for this item, but falls significantly short of portfolio-ready expectations.* |
| **2** | *Project exceeds the minimum requirements for this item, but falls short of portfolio-ready expectations.* |
| **3** | *Project meets or exceeds portfolio-ready expectations; demonstrates a thorough understanding of every outlined consideration.* |


### The Data Science Process

**Problem Statement**
- Is it clear what the goal of the project is?
- What type of model will be developed?
- How will success be evaluated?
- Is the scope of the project appropriate?
- Is it clear who cares about this or why this is important to investigate?
- Does the student consider the audience and the primary and secondary stakeholders?

**Data Collection**
- Was enough data gathered to generate a significant result?
- Was data collected that was useful and relevant to the project?
- Was data collection and storage optimized through custom functions, pipelines, and/or automation?
- Was thought given to the server receiving the requests such as considering number of requests per second?

**Data Cleaning and EDA**
- Are missing values imputed/handled appropriately?
- Are distributions examined and described?
- Are outliers identified and addressed?
- Are appropriate summary statistics provided?
- Are steps taken during data cleaning and EDA framed appropriately?
- Does the student address whether or not they are likely to be able to answer their problem statement with the provided data given what they've discovered during EDA?

**Preprocessing and Modeling**
- Is text data successfully converted to a matrix representation?
- Are methods such as stop words, stemming, and lemmatization explored?
- Does the student properly split and/or sample the data for validation/training purposes?
- Does the student test and evaluate a variety of models to identify a production algorithm (**AT MINIMUM:** two models)?
- Does the student defend their choice of production model relevant to the data at hand and the problem?
- Does the student explain how the model works and evaluate its performance successes/downfalls?

**Evaluation and Conceptual Understanding**
- Does the student accurately identify and explain the baseline score?
- Does the student select and use metrics relevant to the problem objective?
- Does the student interpret the results of their model for purposes of inference?
- Is domain knowledge demonstrated when interpreting results?
- Does the student provide appropriate interpretation with regards to descriptive and inferential statistics?

**Conclusion and Recommendations**
- Does the student provide appropriate context to connect individual steps back to the overall project?
- Is it clear how the final recommendations were reached?
- Are the conclusions/recommendations clearly stated?
- Does the conclusion answer the original problem statement?
- Does the student address how findings of this research can be applied for the benefit of stakeholders?
- Are future steps to move the project forward identified?


### Organization and Professionalism

**Project Organization**
- Are modules imported correctly (using appropriate aliases)?
- Are data imported/saved using relative paths?
- Does the README provide a good executive summary of the project?
- Is markdown formatting used appropriately to structure notebooks?
- Are there an appropriate amount of comments to support the code?
- Are files & directories organized correctly?
- Are there unnecessary files included?
- Do files and directories have well-structured, appropriate, consistent names?

**Visualizations**
- Are sufficient visualizations provided?
- Do plots accurately demonstrate valid relationships?
- Are plots labeled properly?
- Are plots interpreted appropriately?
- Are plots formatted and scaled appropriately for inclusion in a notebook-based technical report?

**Python Syntax and Control Flow**
- Is care taken to write human readable code?
- Is the code syntactically correct (no runtime errors)?
- Does the code generate desired results (logically correct)?
- Does the code follows general best practices and style guidelines?
- Are Pandas functions used appropriately?
- Are `sklearn` and `NLTK` methods used appropriately?

**Presentation**
- Is the problem statement clearly presented?
- Does a strong narrative run through the presentation building toward a final conclusion?
- Are the conclusions/recommendations clearly stated?
- Is the level of technicality appropriate for the intended audience?
- Is the student substantially over or under time?
- Does the student appropriately pace their presentation?
- Does the student deliver their message with clarity and volume?
- Are appropriate visualizations generated for the intended audience?
- Are visualizations necessary and useful for supporting conclusions/explaining findings?



