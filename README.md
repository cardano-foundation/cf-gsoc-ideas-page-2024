# Google Summer of Code 2024 Ideas 🎉

This page showcases project ideas that align seamlessly with our Roadmap and are an ideal fit for GSOC '24. We aim to offer valuable insights into the necessary skillset and prerequisites, along with expectations for learning throughout the project. In addition to providing a project name and a concise descriptive abstract, we've included an assessment of general difficulty (assuming you meet the requirements) and project size. You will find the project list below. The sections represent the project titles, and the subsections are structured as follows:

| Subsection                            | Meaning                 | Values                                |
|---------------------------------------|-------------------------|---------------------------------------|
| Your Mission                          | Brief Overview             | `Free-form text`                           |
| Skills required                       | Things you already know | `List of skills and technologies`     |
| You'll know those things after summer | Things you will learn   |  `List of skills and technologies`    |
| Difficulty                            | Difficulty ranges from a significant workload but straightforward implementation (Easy) to a research-oriented task with an unpredictable outcome (Challenging) | `Easy, Medium, Hard, Challanging` |
| Size                                  | Consider the project's potential output size: whether it will be a Jupyter notebook (S-M), a library, or a standalone application (L-XL) | `S, M, L, XL` |

For example, some projects may involve research tasks resulting in a small but significant output, categorized as both `Challenging` in Difficulty and `S` in Size. On the other hand, there might be projects with a well-defined vision, but requires a lot of time for implementation and testing, falling into the `XL` Size category but with an `Easy` difficulty level. In essence, Difficulty reflects the time spent for thinking, while Size corresponds to the time invested in coding.

## 👉 Untyped Plutus Core Viewer, AKA Understandable Decompiled Smart Contracts

### 🚣 Your Mission

UPLC (Untyped Plutus Core) is executed on-chain and serves as the foundational layer for Cardano smart contracts. High-level languages like Aiken or Helios compile to UPLC. While it's possible to decode the binary (flat) encoded UPLC contract into its text representation, the resulting tree structure is not particularly readable. The objective of this project is to discover a more user-friendly representation of the decoded structure. We welcome rule-based or machine learning solutions that not only transform the binary form into text but also render it in a readable format, making it accessible for e.g. TypeScript developers to comprehend the actual functionality of a contract. We would like you to implement the viewer within a standalone React (Vite.js) app and also export the viewer component itself as a reusable component to npm. This allows other applications within the Cardano ecosystem to utilize its features.

<img src="https://github.com/cardano-foundation/cf-gsoc-ideas-page-2024/assets/1525818/37084b72-2340-4a58-82e6-da34870fed37" height="360">

**Source: https://aiken-lang.org/uplc**

### 🏄 Skills required

Typescript, React.js, General understanding of Compliers and Decompliers

### 🐋 You'll know those things after summer

Cardano Smart Contracts, Plutus Core, Aiken

### 🏋️ Difficulty

Medium

### 👕 Size

L - XL

## 👉 Cardano Peer Connect (CIP-0045) Improvements

### 🚣 Your Mission

[CIP-0045](https://github.com/cardano-foundation/CIPs/tree/master/CIP-0045) introduces a method for setting up a peer-to-peer communication between two browser windows on different devices, eliminating the need for a central signaling server to exchange their IP addresses. This technique allows for the injection of an API (CIP-0030) from one browser (a wallet) to another (a DApp), enabling seamless and lightweight mobile support. To resolve their deep IPs behind different NATs, this approach uses a list of public WebTorrent trackers for peer discovery. However, in many scenarios, when the user is on a mobile device and aims to connect a wallet to a DApp in a browser on the same device, or in another situation where the user is on the same local network and wants to link the wallet on a phone to a DApp on the PC, the use of a torrent tracker becomes unnecessary due to the absence of NAT involvement. Furthermore, there's currently a bit of a hassle in switching between a browser-based wallet and a website, for instance, to sign a message. The mission of this project would be to investigate both topics: situation-dependent peer discovery and enhanced usability. You can explore a demo setup in the open-source repository [available here](https://github.com/fabianbormann/cip-0045-demo-implementation)https://github.com/fabianbormann/cip-0045-demo-implementation.

### 🏄 Skills required

Typescript, React.js, Ionic, Node.js

### 🐋 You'll know those things after summer

WebTorrent, CIP-0030 (Cardano dApp-Wallet Web Bridge), Firebase Cloud Messaging SDK

### 🏋️ Difficulty

Hard

### 👕 Size

L - XL

## 👉 Smart Contract Classificator

### 🚣 Your Mission

At the moment, figuring out the purpose of a smart contract on Cardano only based on hashes and binary data is quite challenging. However, there are always identifiable patterns. Have you ever wondered how many smart contracts are actually being utilized for financial purposes? Is Cardano positioning itself as the go-to blockchain for gaming? What about smart contracts in supply chain scenarios, voting mechanisms, or even for distributing art and music? The truth is, no one really knows... yet.

This mission involves developing a smart contract classifier using a combination of machine learning, statistics, and various conditions. From Convolutional Networks to Gradient Boosting Decision Trees, and even manual feature engineering – everything is on the table. The goal is to design an algorithm capable of taking a smart contract transaction and providing probabilities for different use-case labels.

Whether it's addresses, reference scripts, or reference datums, we are confident that you'll create a tool that can answer the questions mentioned above. To support you in this venture, we'll assign you a mentor with previous experience as a machine learning engineer. This mentor will provide you with ground truth data, guide you on how to find it, and offer deeper insights into the world of Cardano. Towards the end of this journey, our plan is to apply your algorithm to all the on-chain contracts to create a meaningful report.

### 🏄 Skills required

Python, Scala, Statstics, Machine Learning (basics), Smart Contracts under Cardano (beginner level)

### 🐋 You'll know those things after summer

Classification algorithms, Data Science, Cardano Smart Contracts, deep insights in how Cardano actually works

### 🏋️ Difficulty

Challenging 

### 👕 Size

M

## 👉 Enhanced Cardano Asset API Service

### 🚣 Your Mission

Your challenge is to elevate the utility of the Cardano testnet by developing a versatile API service. This service will automate the minting and distribution of a diverse range of Cardano blockchain assets, including NFTs and native tokens, to specified payment addresses. This project is a significant step beyond the current capabilities of the **Cardano faucet**, which is limited to dispensing Ada. By integrating various asset types defined in the Cardano Improvement Proposals (CIPs), such as CIP-25 (Media Token Metadata Standard) and CIP-54 (Cardano Smart NFTs), you will be creating a tool that is indispensable for developers. This API will serve as a critical resource, providing them with a variety of test assets to enhance the development, testing, and optimization of wallets, blockchain explorers, and other applications/dApps. Your work will play a pivotal role in simulating real-world asset handling, crucial for the rigorous testing and preparation of applications before their deployment in production environments.

### 🏄 Skills Required

- Proficiency in Javascript(recommended) or Java, for minting assets.
- Experience with RESTful API development.
- Familiarity with blockchain technology, specifically Cardano's ecosystem. 
- Understanding of Cardano's native tokens and NFTs as per CIPs (like CIP-25, CIP-54).

### 🐋 You'll Know Those Things After Summer

In-depth knowledge of Cardano's blockchain and asset standards
Experience in developing and deploying scalable blockchain APIs
Expertise in integrating diverse blockchain assets into applications

### 🏋️ Difficulty

Medium – This project involves not only the technical aspects of API development and blockchain integration but also requires a deep understanding of the Cardano blockchain's native asset standards.

### 👕 Size

M - L – The project's output will be a fully functional API service capable of handling multiple asset types, requiring significant coding and testing.

### 🌍 Importance of Testnets in Blockchain Development

The importance of testnets in blockchain development cannot be overstated. Testnets provide a sandbox environment where developers can experiment and test their applications without risking real funds or impacting the main blockchain. They are crucial for:

- Ensuring the security and stability of new features before they are deployed on the mainnet.
- Allowing developers to test the integration of different asset types and ensure compatibility with various wallet and explorer applications.
- Facilitating the development and testing of smart contracts under real-world conditions without the associated risks.
  
This challenge, therefore, not only enhances the capabilities of the Cardano testnet environment but also significantly contributes to the broader development ecosystem, enabling developers to build more robust, diverse, and secure applications on the Cardano blockchain.
