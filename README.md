# Google Summer of Code 2024 Ideas

This page showcases project ideas that align seamlessly with our Roadmap and are an ideal fit for GSOC '24. We aim to offer valuable insights into the necessary skillset and prerequisites, along with expectations for learning throughout the project. In addition to providing a project name and a concise descriptive abstract, we've included an assessment of general difficulty (assuming you meet the requirements) and project size

## UPLC Viewer

UPLC (Untyped Plutus Core) is executed on-chain and serves as the foundational layer for Cardano smart contracts. High-level languages like Aiken or Helios compile to UPLC. While it's possible to decode the binary (flat) encoded UPLC contract into its text representation, the resulting tree structure is not particularly readable. The objective of this project is to discover a more user-friendly representation of the decoded structure. We welcome rule-based or machine learning solutions that not only transform the binary form into text but also render it in a readable format, making it accessible for e.g. TypeScript developers to comprehend the actual functionality of a contract. We would like you to implement the viewer within a standalone React (Vite.js) app and also export the viewer component itself as a reusable component to npm. This allows other applications within the Cardano ecosystem to utilize its features.

### Tech you need to know	

Typescript, React.js, General understanding of Compliers and Decompliers

### Tech you will learn	

Cardano Smart Contracts, Plutus Core, Aiken

### Difficulty

Medium

### Size

L - XL
