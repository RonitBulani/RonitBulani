# Hi, I'm Ronit

I'm a Lancaster University Data Science graduate based in Manchester. Most of my recent projects have involved Python, machine learning and working out how to make research useful beyond a notebook.

Before my MSc, I worked in marketing strategy and performance marketing. That experience has stayed with me: I like to understand the problem first, choose methods that fit it, and be able to explain what the results actually mean.

## Projects I've worked on

### [ParliamentAI — GraphRAG for UK Parliamentary Debates](https://github.com/RonitBulani/graphrag-uk-parliament)

This started as a research project exploring whether a knowledge graph could help retrieve evidence for questions spanning multiple parliamentary speeches. I worked with **39,423 Brexit-related speeches**, built a graph and vector-based retrieval pipeline, and compared GraphRAG with a hybrid RAG baseline on **50 questions**. GraphRAG retrieved a wider range of speakers, although the results were mixed across the other evaluation metrics.

I later turned the research into **ParliamentAI**, a local application built with FastAPI and React. It lets users ask questions, inspect the speeches behind an answer, filter the evidence and save or export conversations. I also added Docker support and GitHub Actions checks.

[Project and screenshots](https://github.com/RonitBulani/graphrag-uk-parliament) · [v1.0.0 release](https://github.com/RonitBulani/graphrag-uk-parliament/releases/tag/v1.0.0)

### [Byzantine-Resilient Communication for Multi-Agent RL](https://github.com/RonitBulani/byzantine-resilient-marl-comms)

This was part of a five-person MSc project on cooperative multi-agent reinforcement learning. We studied what happens when agents rely on messages from other agents and some of those messages are unreliable. I led the **Byzantine attack and communications work**, implementing random-noise, misdirection, spoofing and silence attacks, alongside broadcast, gossip, trimmed-mean and reputation-based communication methods.

The wider team evaluated the system over **30,000 episodes**. One interesting finding was how strongly losing messages could affect performance: in the narrow-visibility setting, silence reduced the recorded MAPPO capture rate by **48.3 percentage points** at a 50% Byzantine fraction. The experiment used a shared channel with access to the true target position, so these findings are about robustness to corrupted communication under that setup—not fully local sensing.

The repository contains the communication components I built and links back to the original team project. [Implementation and limitations](https://github.com/RonitBulani/byzantine-resilient-marl-comms/blob/main/docs/IMPLEMENTATION_LIMITATION.md)

### [Amazon Product Analytics — PostgreSQL and Clustering](https://github.com/RonitBulani/amazon-product-clustering-postgres)

In another university group project, I focused on making a large collection of Amazon product and review data easier to explore and analyse. My contribution covered **exploratory data analysis**, looking at missing values, duplicates, pricing, ratings and category patterns, followed by work in **PostgreSQL** to organise users, products and reviews. I wrote queries and added indexes for common lookups and full-text search.

I also compared **K-Means, Bisecting K-Means and Gaussian Mixture Models** for product clustering, using text embeddings and numeric features, then explored the groups through dimensionality reduction and visualisations. K-Means gave the strongest results on the recorded internal diagnostics, although the methods used different distance assumptions, so the comparison has limits.

The linked repository includes the notebooks, results and an explanation of exactly which parts were my work. [Clustering results](https://github.com/RonitBulani/amazon-product-clustering-postgres/blob/main/results/RESULTS.md)

## Dissertation with Network Rail

For my MSc dissertation, I worked with **Network Rail** on making it easier to update the deterioration matrices used in drainage asset planning. These matrices estimate how an asset's condition may change over time, and the aim was to make it more practical to recalculate them as new inspection data becomes available.

I implemented an established **continuous-time Markov modelling** method in Python and developed a workflow for preparing inspection histories, estimating condition transitions and producing updated matrices. A significant part of the work was checking how reliable those estimates were. I used simulations with known outcomes, tested predictions against later inspection records, and added diagnostics and uncertainty checks.

I also investigated how deterioration patterns varied over time, across materials and between structural and service condition. The resulting Python matrices were accepted by Network Rail for integration into its asset-planning workflow.

The project involved internal industry data, so the full dataset and code are not published here.

## What I use

I work mainly with **Python, pandas, NumPy, SciPy and SQL/PostgreSQL**. Depending on the project, I've also used **scikit-learn, NetworkX, ChromaDB, FastAPI, React, Docker and GitHub Actions**.

I'm looking for opportunities in the UK where I can work on **AI, data science, analytics or related technical and business problems**.
