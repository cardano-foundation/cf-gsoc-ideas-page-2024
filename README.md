# Google Summer of Code 2024 Ideas 🎉

This page showcases project ideas that align seamlessly with our Roadmap and are an ideal fit for GSOC '24. We aim to offer valuable insights into the necessary skillset and prerequisites, along with expectations for learning throughout the project. In addition to providing a project name and a concise descriptive abstract, we've included an assessment of general difficulty (assuming you meet the requirements) and project size

## 👉 UPLC Viewer

### 🚣 Your Mission

UPLC (Untyped Plutus Core) is executed on-chain and serves as the foundational layer for Cardano smart contracts. High-level languages like Aiken or Helios compile to UPLC. While it's possible to decode the binary (flat) encoded UPLC contract into its text representation, the resulting tree structure is not particularly readable. The objective of this project is to discover a more user-friendly representation of the decoded structure. We welcome rule-based or machine learning solutions that not only transform the binary form into text but also render it in a readable format, making it accessible for e.g. TypeScript developers to comprehend the actual functionality of a contract. We would like you to implement the viewer within a standalone React (Vite.js) app and also export the viewer component itself as a reusable component to npm. This allows other applications within the Cardano ecosystem to utilize its features.

### 🏄 Skills required

Typescript, React.js, General understanding of Compliers and Decompliers

### 🐋 You'll know those things after summer

Cardano Smart Contracts, Plutus Core, Aiken

### 🏋️ Difficulty

Medium

### 👕 Size

L - XL

## 👉 CIP-0045 Improvements 

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
