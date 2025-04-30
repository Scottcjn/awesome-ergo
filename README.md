# Awesome Ergo

A curated list of awesome projects, tools, libraries, and resources for the Ergo Blockchain ecosystem.

**Contributing:** Please feel free to open a Pull Request on GitHub to add or update projects! Ensure added items are active, relevant, and have a working URL. Contributions to the documentation itself can be made at [ergoplatform/ergodocs](https://github.com/ergoplatform/ergodocs). You can find this list's source at [ergoplatform/awesome-ergo](https://github.com/ergoplatform/awesome-ergo).

## Table of Contents

- [Awesome Ergo](#awesome-ergo)
  - [Table of Contents](#table-of-contents)
  - [Core Infrastructure](#core-infrastructure)
    - [Nodes](#nodes)
    - [Oracles](#oracles)
    - [Bridges](#bridges)
    - [Frameworks](#frameworks)
  - [Wallets](#wallets)
    - [Browser \& Desktop](#browser--desktop)
    - [Mobile](#mobile)
    - [Hardware Wallet Support](#hardware-wallet-support)
    - [Utilities \& Recovery](#utilities--recovery)
  - [SDKs \& Libraries](#sdks--libraries)
    - [Primary SDKs](#primary-sdks)
    - [Core Libraries \& Cryptography](#core-libraries--cryptography)
    - [Language Bindings \& Wrappers](#language-bindings--wrappers)
    - [Community SDKs/Libraries](#community-sdkslibraries)
  - [Development Tooling](#development-tooling)
    - [Smart Contracts \& ErgoScript](#smart-contracts--ergoscript)
    - [Frameworks \& Templates](#frameworks--templates)
    - [Utilities \& CLI](#utilities--cli)
    - [Node Interaction \& APIs](#node-interaction--apis)
    - [Testing \& Debugging](#testing--debugging)
    - [Examples \& Snippets](#examples--snippets)
  - [DeFi \& dApps](#defi--dapps)
    - [DEXs \& Swaps](#dexs--swaps)
    - [Stablecoins \& Lending](#stablecoins--lending)
    - [Launchpads](#launchpads)
    - [Identity \& DNS](#identity--dns)
    - [Privacy](#privacy)
    - [Gaming \& Metaverse](#gaming--metaverse)
    - [DAO Frameworks](#dao-frameworks)
    - [Other dApps \& Services](#other-dapps--services)
  - [NFT Ecosystem](#nft-ecosystem)
    - [Marketplaces \& Auctions](#marketplaces--auctions)
    - [Minting \& Utilities](#minting--utilities)
    - [NFT Projects](#nft-projects)
  - [Mining](#mining)
    - [Pools](#pools)
    - [Software](#software)
    - [Utilities \& Tooling](#utilities--tooling)
    - [Smart Pooling](#smart-pooling)
  - [Standards (EIPs)](#standards-eips)
  - [Explorers \& Dashboards](#explorers--dashboards)
  - [Analytics](#analytics)
  - [Community \& Resources](#community--resources)
    - [Information Hubs](#information-hubs)
    - [Contribution Platforms](#contribution-platforms)
    - [Education \& Tutorials](#education--tutorials)
    - [Papers \& Specifications](#papers--specifications)
    - [Utilities](#utilities)

---

## Core Infrastructure

### Nodes

*   [Reference Client (Node)](https://github.com/ergoplatform/ergo): The official Ergo node implementation. [`Scala`] [Status: Active]
*   [Ergode](https://github.com/ross-weir/ergode): Ergo node implementation in TypeScript (experimental). [`TS`]

### Oracles

*   [Oracle Core](https://github.com/ergoplatform/oracle-core): Core implementation for Ergo oracle pools V2. [`Rust`] [Status: Active]
    *   [Oracle Pool Bootstrap](https://github.com/ergoplatform/oracle-core/tree/master/oracle-pool-bootstrap): Scripts and configs to bootstrap new oracle pools.
    *   [Connector Library](https://github.com/ergoplatform/oracle-core/tree/master/connectors/connector-lib): Library for connecting data sources to the oracle core.
    *   [How to Bootstrap Oracles Guide](https://github.com/ergoplatform/oracle-core/blob/develop/docs/how_to_bootstrap.md): Guide for setting up oracle pools using the core library.
*   [EIP-23 Oracle Pools 2.0](https://github.com/ergoplatform/eips/pull/41): Specification for the improved V2 oracle pool protocol.
*   [Ergo Oracles V1 Overview](https://github.com/Emurgo/Emurgo-Research/blob/master/oracles/Oracle-Pools.md): Document explaining the Oracle Pool V1 design.
*   [Ergo Easy Oracle](https://github.com/reqlez/ergo-easy-oracle): Docker setup for simplifying oracle pool deployment. [`Docker`]
*   [Oracle Core ETH Connector Fork](https://github.com/Luivatra/oracle-core/tree/eth-connector): Fork exploring ETH data connection. [`Rust`]
*   [Sininen Taivas Ergo Oracle](https://github.com/sininen-taivas/ergo-oracle): CLI tool for launching oracles. [`Go`?]
*   [Oracle Pool V1 Kiosk Example](https://github.com/scalahub/Kiosk/tree/master/src/test/scala/kiosk/oraclepool/v4a): Kiosk tests for Oracle Pool V1. [`Scala`]
*   [Oracle Pool Stats Backend (Delphi)](https://github.com/thedelphiproject/ergo-oracle-stats-backend): Backend for Oracle Pool statistics.
*   [Oracle Pool Tools JS (Delphi)](https://github.com/thedelphiproject/ergo-oracle-tools-js): JavaScript tools for interacting with Oracle Pools. [`JS`]

### Bridges

*   [Rosen Bridge](https://rosen.tech/): The primary cross-chain bridge protocol for Ergo. [GitHub Org](https://github.com/rosen-bridge) [Status: Active] [Live]
    *   [Rosen Contracts](https://github.com/rosen-bridge/contract): Smart contracts for the Rosen bridge. [`JS/TS`, `Scala`]
    *   [Rosen Operation/Watcher](https://github.com/rosen-bridge/operation): Watcher and guard operation software. [`Scala`?]
    *   [Rosen Utils CLI](https://github.com/rosen-bridge/utils/tree/dev/packages/cli): CLI tool for Rosen bridge operations. [`TS`?]
    *   [Rosen Docker Deployment Guide](https://github.com/rosen-bridge/operation/blob/dev/docs/watcher/deploy-docker.md): Guide for deploying Rosen watchers using Docker.

### Frameworks

*   [Scorex](https://github.com/scorexfoundation/scorex): The modular blockchain framework underlying Ergo. [`Scala`]

## Wallets

### Browser & Desktop

*   [Nautilus Wallet](https://nautilus-wallet.io/): Feature-rich browser extension wallet supporting dApp Connector. [GitHub](https://github.com/nautls/nautilus-wallet) [`JS/TS`] [Status: Active] [Live]
*   [SAFEW (Secure Asset Funk Engine Wallet)](https://chrome.google.com/webstore/detail/safew/lmjcdljhgidjbcpdkfknpfknbbkfpogg): Browser extension wallet supporting dApp Connector. [GitHub](https://github.com/ThierryM1212/SAFEW) [`JS/TS`] [Status: Active] [Live]
*   [Satergo](https://satergo.com/): Desktop wallet focused on security and privacy, includes a full node. [GitHub](https://github.com/Satergo/Satergo) [`Java`] [Live]

### Mobile

*   [Minotaur Wallet](https://minotaur-wallet.io/): Mobile wallet for Android and iOS with multi-sig support. [GitHub](https://github.com/minotaur-ergo/minotaur-wallet) [`JS/TS`] [Status: Active] [Live]
    *   [Multi-Sig Coordination Server](https://github.com/minotaur-ergo/Minotaur-Signing-Server) / [Alternative](https://github.com/lazypinkpatrick/cosigning-server): Backend server for coordinating multi-signature operations.
*   [Ergo Mobile Wallet (Android)](https://play.google.com/store/apps/details?id=org.ergoplatform.android): Official Android wallet. [GitHub](https://github.com/ergoplatform/ergo-wallet-app) [`Kotlin`] [Status: Active] [Live]
*   [Ergo Mobile Wallet (iOS)](https://apps.apple.com/us/app/ergo-wallet-app/id1569044501): Official iOS wallet. [GitHub](https://github.com/ergoplatform/ergo-wallet-app) [`Swift`] [Status: Active] [Live]
*   [Ergo Light Client (iOS Beta)](https://github.com/bjenkinsgit/ErgoIOSLiteClient): Community iOS light client (Requires a full node). [`Swift`] [Status: Beta]

### Hardware Wallet Support

*   [Ledger](https://github.com/tesseract-one/ledger-app-ergo): Ledger hardware wallet app for Ergo. [`C`] [Status: Active] [Live]
    *   [LedgerJS Bindings](https://github.com/anon-br/ledgerjs-hw-app-ergo): JavaScript library for interacting with the Ledger Ergo app. [`JS`]
    *   [Ledger4j Bindings](https://github.com/aionnetwork/ledger4j): Java library potentially usable for Ledger interaction. [`Java`]
    *   [Ledger Core Lib](https://github.com/LedgerHQ/lib-ledger-core): Ledger's core library used internally. [`C++`]

### Utilities & Recovery

*   [Ergo Paper Wallet Generator](https://anon-br.github.io/ergo-paper-wallet/): Simple web tool to generate paper wallets. [GitHub](https://github.com/anon-br/ergo-paper-wallet) [`JS/TS`] [Live]
*   [Yoroi Ergo Wallet Recovery Tool](https://github.com/satsen/yoroi-ergo-wallet-recover): Tool to recover funds from old Yoroi Ergo wallets. [`Java`]
*   [Stealth Address Generator](https://ergomixer.github.io/stealth/): Web tool for generating stealth addresses compatible with ErgoMixer.
*   [Cold Wallet Setup Guide (Wiki)](https://github.com/ergoplatform/ergo-wallet-app/wiki/Cold-wallet): Guide on setting up and using cold wallets with the official mobile apps.
*   [Ergo Poor Man's Wallet (EPMW)](https://github.com/epmw/epmw): DIY ultra-low-cost hardware wallet solution (ErgoHack VII). [`Hardware`]

## SDKs & Libraries

### Primary SDKs

*   [AppKit](https://github.com/ergoplatform/ergo-appkit): A Java/Scala library for building Ergo applications and off-chain code. [`Java`, `Scala`] [Status: Active]
*   [Fleet SDK](https://fleet-sdk.github.io/docs/): A JavaScript/TypeScript SDK for building web-based Ergo dApps. [GitHub](https://github.com/fleet-sdk) [`JS/TS`] [Status: Active]
*   [Sigma-Rust](https://github.com/ergoplatform/sigma-rust/): Core Ergo primitives, cryptography, and protocol serialization in Rust. The foundation for many Ergo tools and SDKs. [`Rust`] [Status: Active]

### Core Libraries & Cryptography

*   [Sigmastate Interpreter](https://github.com/ScorexFoundation/sigmastate-interpreter): The core interpreter and type system for ErgoScript. [`Scala`, `ErgoScript`] [Status: Active]
*   [Scrypto](https://github.com/input-output-hk/scrypto/): Cryptographic primitives library (hashes, signatures, authenticated data structures) used by Ergo. [`Scala`]
*   [Scorex Util](https://github.com/ScorexFoundation/scorex-util): Utility classes used by Scorex projects. [`Scala`]
*   [Debox](https://github.com/ScorexFoundation/debox): Efficient, mutable and immutable Boxes for primitive types. [`Scala`]
*   [BouncyCastle JS](https://github.com/aslesarenko/bouncycastle-js): BouncyCastle crypto library compiled for JavaScript (used by older SigmaJS?). [`JS`]
*   [Scorex Crypto AVLTree](https://github.com/knizhnik/scorex_crypto_avltree): Rust AVL Tree implementation used by sigma-rust. [Paper](https://github.com/knizhnik/scorex_crypto_avltree/blob/main/crypto_avltree.md) [`Rust`]

### Language Bindings & Wrappers

*   [ErgoLib (sigma-rust)](https://github.com/ergoplatform/sigma-rust/tree/develop/ergo-lib): Rust crate providing high-level abstractions over ErgoTree IR. [Docs](https://docs.rs/ergo-lib/) [`Rust`]
*   [ergo-lib-wasm](https://github.com/ergoplatform/sigma-rust/tree/develop/bindings/ergo-lib-wasm): WASM bindings for sigma-rust, enabling use in JS/TS. [NPM (Browser)](https://www.npmjs.com/package/ergo-lib-wasm-browser) | [NPM (NodeJS)](https://www.npmjs.com/package/ergo-lib-wasm-nodejs) [`JS/TS`, `Rust`]
*   [ergo-lib-jni](https://github.com/ergoplatform/sigma-rust/tree/develop/bindings/ergo-lib-jni): JNI bindings for sigma-rust (for JVM languages). [Docs](https://docs.rs/ergo-lib-jni/) [`Java`, `Rust`]
*   [ergo-lib-c](https://github.com/ergoplatform/sigma-rust/tree/develop/bindings/ergo-lib-c): C bindings for sigma-rust. [Docs](https://docs.rs/ergo-lib-c/) [`C`, `Rust`]
*   [ergo-lib-python](https://github.com/ergoplatform/sigma-rust/tree/develop/bindings/ergo-lib-python): Python bindings for sigma-rust. [PyPI](https://pypi.org/project/ergo-lib/) [`Python`, `Rust`]
*   [ergo-lib-go](https://github.com/sigmaspace-io/ergo-lib-go): Go bindings for sigma-rust (via C bindings). [Docs](https://pkg.go.dev/github.com/ergoplatform/ergo-lib-go) [`Go`, `C`, `Rust`] (Community Maintained)
*   [Ergo Wallet Core (JVM)](https://mvnrepository.com/artifact/org.ergoplatform/ergo-wallet): Wallet-related logic extracted from the reference node. [Source](https://github.com/ergoplatform/ergo/tree/master/ergo-wallet) [`Java`]

### Community SDKs/Libraries

*   [FleetSharp](https://github.com/pulsarz/FleetSharp): A C# library for building transactions, inspired by Fleet SDK. [`C#`]
*   [Ergpy](https://github.com/mgpai22/ergpy): Python wrapper using JPype for interacting with Ergo (AppKit based). [`Python`, `Java`]
*   [ergo-golang](https://github.com/azhiganov/ergo-golang): Early-stage Go library for Ergo. [`Go`]
*   [sigma_rb](https://github.com/thedlop/sigma_rb): Ruby bindings for sigma-rust (via C bindings). [`Ruby`, `C`, `Rust`]
*   [sigma-rust-mini](https://github.com/aslesarenko/sigma-rust-mini): Minified version of sigma-rust, useful for constrained environments. [`Rust`]
    *   [No-Std Fork](https://github.com/Alesfatalis/sigma-rust-mini/tree/no_std): Fork focusing on `no_std` compatibility (e.g., for hardware wallets).
*   [ergo-python-appkit](https://github.com/ergo-pad/ergo-python-appkit): Alternative Python wrapper for Ergo AppKit using JPype. [`Python`, `Java`]
*   [ogre](https://github.com/ross-weir/ogre): TypeScript Ergo node client library targeting web/browser & Deno/native platforms. [`JS/TS`]
*   [ergo_client](https://github.com/ross-weir/ergo_client): Rust library containing HTTP clients for various Ergo applications. [`Rust`]
*   [sigma-builders](https://github.com/GuapSwap/sigma-builders): Protocol abstractions built on AppKit for easier dApp development in Scala. [`Scala`]
*   [eip12-types](https://github.com/capt-nemo429/eip12-types): TypeScript library providing static types for the EIP-12 dApp Connector protocol. [`TS`]
*   [GetBlok Plasma](https://github.com/GetBlok-io/GetBlok-Plasma): Library built on AppKit to simplify integrating AVL Trees (Plasma L2 scaling) into off-chain code. [`Scala`]
*   [sigmajs-crypto-facade](https://github.com/anon-br/sigmajs-crypto-facade): Project aiming to replace BouncyCastle dependencies in SigmaJS builds. [`JS/TS`]
*   [ScalaSigmaParticle](https://github.com/dzyphr/ScalaSigmaParticle): Framework based on Ergpy for cross-chain pipelines. [`Python`]
*   [dApp Connector React Package (NightOwl)](https://github.com/nightowlcasino/dApp-connector-react-package): React package for EIP-12 dApp Connector. [`JS/TS`, `React`]
*   [Ergo SDK JS (ErgoLabs)](https://github.com/ergolabs/ergo-sdk-js): Community JS SDK using Wasm bindings. [`JS/TS`, `Wasm`]

## Development Tooling

### Smart Contracts & ErgoScript

*   [Sigmastate Interpreter](https://github.com/ScorexFoundation/sigmastate-interpreter): The core interpreter and type system for ErgoScript. [`Scala`, `ErgoScript`]
*   [Ergoscript Compiler (Rust)](https://github.com/ergoplatform/sigma-rust/tree/develop/ergoscript-compiler): Rust implementation of the ErgoScript compiler. [`Rust`]
*   [Ergoscript Compiler (Scala)](https://github.com/ergoplatform/ergoscript-compiler): Scala CLI tool to compile ErgoScript source code. [`Scala`]
*   [Ergo Playgrounds](https://github.com/ergoplatform/ergo-playgrounds): Scala-based playgrounds for developing and testing ErgoScript contracts and off-chain code. [`Scala`]
*   [VSCode ErgoScript Language Support](https://marketplace.visualstudio.com/items?itemName=ergoscript.ergoscript-language-support): Syntax highlighting for ErgoScript in VSCode. [Source](https://github.com/GuapSwap/vscode-ergoscript-language-support)
*   [escript.online](https://escript.online/): Online ErgoScript editor and playground. [GitHub](https://github.com/SavonarolaLabs/escript-online) [`JS/TS`]
*   [FlowcardLib](https://github.com/lucagdangelo/flowcardLib): Library of ErgoScript contract templates and examples. [`ErgoScript`]
*   [ergo-script-re](https://github.com/ross-weir/ergo-script-re): Libraries for ErgoScript reverse engineering and analysis, including pseudo-code generation. [`Rust`]
*   [ergo-castanet](https://github.com/iandebeer/ergo-castanet): Tooling for ErgoScript development using Dhall for configuration. [`Dhall`, `Scala`]
*   [Plutomonkey](https://wallet.plutomonkey.com/): Web tool for compiling ErgoScript (and Plutus).
*   [Ergo Playground (Scastie)](https://scastie.scala-lang.org/ergoplatform): Online Scala/ErgoScript playground (used in ergoscript-by-example).
*   [KioskWeb](https://github.com/scalahub/KioskWeb): Web interface for the Kiosk framework. [`Scala`, `JS/TS`?]

### Frameworks & Templates

*   [Headless dApp Framework](https://github.com/ergoplatform/ergo-headless-dapp-framework): Rust framework for developing portable off-chain dApp logic following EIP-6. [`Rust`]
*   [Kiosk](https://github.com/scalahub/Kiosk): Framework for developing secure dApps (Archived, but influential). [`Scala`]
*   [Mosaik](https://github.com/MrStahlfelge/mosaik): Framework for building dApp frontends with native mobile feel (Paused). [`Java`]
*   [Ergo JSON Development Environment (JDE)](https://github.com/ergoplatform/ergo-jde): Framework for developing dApps using JSON configurations. [`JSON`, `Scala`]
*   [ergo-scala-skeleton-app](https://github.com/dav009/ergo-scala-skeleton-app): Skeleton app template for Scala-based Ergo projects. [`Scala`]
*   [ergo-web-template](https://github.com/SavonarolaLabs/ergo-web-template): Web template for Ergo dApps using JS/TS. [`JS/TS`]
*   [ergo-js-template](https://github.com/anon-real/ergo-js-template): Basic JS template for Ergo projects. [`JS/TS`]
*   [Ergo Off-Chain Bot Template](https://github.com/mgpai22/Ergo-OffChain-Bot-Template): Template for building off-chain bots in Scala. [`Scala`]
*   [scala-play-next-ergo](https://github.com/kii-dot/scala-play-next-ergo): Template using Scala Play, Ergo Appkit, and NextJs. [`Scala`, `JS/TS`]
*   [ergo-play-boilerplate](https://github.com/kii-dot/ergo-play-boilerplate): Boilerplate for Scala Play Ergo projects. [`Scala`]
*   [ergo-basic-template](https://github.com/ERGnomes/ergo-basic-template): Basic React template for Ergo dApps. [`JS/TS`, `React`]
*   [Edge](https://github.com/Ergo-Lend/edge): Ergo Development Generics Elements (used by ErgoLend). [`Scala`]
*   [Mosaik Web Executor](https://github.com/MrStahlfelge/mosaik-kt-js): Browser-based executor for the Mosaik UI framework. [`Kotlin`, `JS`]

### Utilities & CLI

*   [ErgoTool](https://github.com/aslesarenko/ergo-tool): A Command Line Interface (CLI) for interacting with the Ergo blockchain via AppKit. [`Scala`]
*   [Ergo Utils (JS)](https://github.com/anon-real/ErgoUtils): Utility library for Ergo in JS/TS. [`JS/TS`]
*   [TokenJay](https://tokenjay.app/): Mobile-friendly web tool for token minting and management. [Website](https://tokenjay.app/)
*   [Yet Another Airdrop Tool (YAAT)](https://github.com/FlyingPig69/YAAT/): Python tool for performing batch transfers/airdrops. [`Python`]
*   [Ergo Node Interface (Rust)](https://github.com/ergoplatform/ergo-node-interface-rust): Rust interface for interacting with the Ergo node API. [`Rust`]
*   [ergo-assembler](https://github.com/anon-real/ergo-assembler): Service/library to help dApps assemble transactions off-chain, bypassing node requirements for users. [`Scala`]
*   [Transaction Builder UI](https://thierrym1212.github.io/txbuilder/): Web UI to manipulate and sign Ergo transaction JSON. [GitHub](https://github.com/ThierryM1212/transaction-builder/) [`JS/TS`]
*   [ErgoSimpleAddresses](https://github.com/kushti/ergo-simple-addresses): Java utilities for working with Ergo addresses. [`Java`]
*   [ErgoUtilsUploadService](https://github.com/arobsn/ErgoUtilsUploadService): Backend service used by ErgoUtils for NFT file uploads. [`C#`]
*   [Ergo Vanity Address Generator](https://github.com/jellymlg/ergo-vanitygen): Generate custom Ergo addresses. [`Scala`]
*   [Ergo Monitoring](https://github.com/SabaunT/ergo-monitoring): Debug service printing useful node and blockchain state information. [`Rust`]
*   [Ergo Faucet](https://github.com/zargarzadehm/ergo-faucet): Simple faucet implementation. [`Scala`]
*   [Chain Name Service](https://github.com/ross-weir/chain-name-service): Experimental name service library/contracts. [`Scala`]
*   [Transaction Group Framework](https://github.com/GetBlok-io/Subpooling#frameworks--abstractions): Framework for managing large interrelated transactions (from GetBlok Subpooling).
*   [ErgoUtilities (Rust)](https://github.com/robkorn/ergo-utilities-rust): Utility library to simplify writing off-chain code in Rust. [`Rust`]
*   [Ergo Setup](https://github.com/abchrisxyz/ergo-setup): Docker-based setup for Node, Explorer & GraphQL. [`Docker`]
*   [Ergo Handshake (Reference)](https://github.com/SabaunT/ergo-handshake): Reference implementation of the Ergo P2P handshake. [`Rust`]
*   [MobilERG](https://github.com/ladopixel/mobilERG): Interact with Ergo via phone calls/SMS. [`Python`]
*   [tERGminal](https://github.com/ladopixel/tERGminal): Interact with Ergo from the terminal. [`Python`]
*   [On-Chain Notifications Service](https://github.com/ergopad/onchain-notifications-service): Scala service for transaction monitoring and event tracking. [`Scala`]
*   [Ergo-node-TUI-installer](https://github.com/Itaggergaard/Ergo-node-TUI-installer): Terminal User Interface installer for Ergo nodes. [`Shell`]
*   [Ergo Synced Node Helper](https://github.com/mgpai22/ergo-synced-node): Helper scripts for setting up a synced node (Mainnet & Testnet). [`Python`, `Shell`]
*   [Ergo Portable Node](https://github.com/ross-weir/ergo-portable): Scripts for a portable Ergo node setup. [`Shell`]
*   [Ergo Nix Toolkit](https://github.com/ergoplatform/ergo-nix): Nix toolkit for Ergo packages and services. [`Nix`]
*   [Ergo Bootstrap](https://github.com/ergoplatform/ergo-bootstrap): Deployment tool using ergo-nix for cluster setup (Node, Explorer, etc.). [`Nix`, `Shell`]
*   [Ergo RPI Scripts](https://github.com/Eeysirhc/ergo-rpi): Scripts/guide for RPi node setup. [`Shell`?]
*   [ErgoScripts (Misc)](https://github.com/glasgowm148/ergoscripts): Miscellaneous community scripts (e.g., nginx config for public node). [`Shell`, `Other`]
*   [ErgoNodeAndroid (Termux)](https://github.com/rustinmyeye/ErgoNodeAndroid): One-click Android node setup app using Termux. [`Shell`, `Android`]

### Node Interaction & APIs

*   [Ergo Node API Swagger UI](http://127.0.0.1:9053/swagger): Interactive API documentation (available when running a node with default settings). [OpenAPI Spec](https://github.com/ergoplatform/ergo/blob/master/src/main/resources/api/openapi.yaml)
*   [Ergo GraphQL](https://github.com/capt-nemo429/ergo-graphql): GraphQL interface for querying Ergo blockchain data. [`JS/TS`]
*   [Rosetta API for Ergo](https://github.com/ross-weir/rosetta-ergo): Implementation of the Rosetta API standard for easier exchange/wallet integration. [`Go`]
*   [Ergo Scanner](https://github.com/ergoplatform/scanner): Framework for scanning the blockchain for specific transactions or events. [`Scala`]
*   [ergo-indexer-rust](https://github.com/darkdrag00nv2/ergo-indexer-rust): Blockchain indexer for Ergo written in Rust. [`Rust`]
*   [Danaides](https://github.com/ergopad/danaides): High-performance blockchain toolkit, including indexing capabilities. [`Python`]
*   [Strainer](https://github.com/dav009/strainer): Listen and pipe Ergo TXs and eUTXOs from a node. [`Rust`]
*   [ergo-node-zmqpub](https://github.com/cruxfinance/ergo-node-zmqpub): Publishes Ergo node events via ZeroMQ for real-time applications. [`Scala`]
*   [Pragmaxim Chain Indexer (Ergo)](https://github.com/pragmaxim-com/chain-indexer/tree/ergo-boxes): Custom indexer implementation. [`Scala`]
*   [Ergonnection](https://github.com/Satergo/Ergonnection): P2P networking library for Ergo. [`Java`]
*   [Ergonode Spyder](https://github.com/chriswill/ergonode-spyder): Network spider to capture node information for analytics. [`C#`]
*   [Ergo Blockchain Scanner (Aragogi)](https://github.com/aragogi/scanner): Alternative blockchain scanner implementation. [`Scala`]

### Testing & Debugging

*   [Contract Testing Framework](https://github.com/anon-real/contract-testing): Framework for testing ErgoScript contracts off-chain using Scala. [`Scala`]
*   [Ergoscript Simulator](https://github.com/spectrum-finance/ergoscript-simulator): Community tool for simulating ErgoScript execution. [`Scala`?]
*   [Ergo Puppet](https://github.com/dav009/ergo-puppet): Tool for off-chain experimentation and unit testing of Ergo contracts, building on Ergo Playgrounds. [`Scala`]
*   [Ergo Test Vectors](https://github.com/ergoplatform/ergo-test-vectors): Standard test vectors for cryptographic primitives and serialization.

### Examples & Snippets

*   [ErgoScript by Example](https://github.com/ergoplatform/ergoscript-by-example): Collection of simple ErgoScript contracts demonstrating various features. [`ErgoScript`]
*   [AppKit Examples](https://github.com/aslesarenko/ergo-appkit-examples): Example code demonstrating usage of Ergo AppKit in multiple languages. [`Java`, `Scala`, `JS`, `Python`, `Ruby`, `C`]
*   [Fleet Examples](https://github.com/fleet-sdk/fleet-by-example): Repository showcasing Fleet SDK usage. [`TS`]
*   [Ergo Contracts](https://github.com/ergoplatform/ergo-contracts): Early examples of Ergo smart contracts with verification tooling. [`Scala`]
*   [SigmaState Interpreter Examples](https://github.com/ScorexFoundation/sigmastate-interpreter/tree/develop/sc/src/test/scala/sigmastate/utxo/examples): Various contract examples within the interpreter tests. [`Scala`]
*   [Kiosk Offchain Examples](https://github.com/scalahub/Kiosk/tree/master/src/test/scala/kiosk/offchain): Examples using the Kiosk off-chain assembler. [`JSON`]
*   [Headless dApp Framework Tutorials](https://github.com/ergoplatform/ergo-headless-dapp-framework/tree/main/tutorials): Tutorials for the headless framework (e.g., Math Bounty dApp). [`Rust`]
*   [Mosaik Examples](https://github.com/MrStahlfelge?tab=repositories&q=mosaik&type=source): Various example apps demonstrating Mosaik UI framework usage. [`Kotlin`, `Java`]
*   [Atomic Swap Example (secp256k1)](https://github.com/dzyphr/atomicswapexample): Example of a 2-party atomic swap. [`Scala`?]
*   [ErgoRaffle Bot (JS)](https://github.com/zkastn/ergo-raffle-bot): JavaScript bot interacting with ErgoRaffle. [`JS`]
*   [Quid Games (ErgoHack)](https://github.com/hypo10use/quid-games): Gaming example from ErgoHack. [`Angular`, `TS`]
*   [NFT Minting for Dummies](https://github.com/lucagdangelo/minting-for-dummies): Basic NFT minting script in Scala. [`Scala`]
*   [Profit Sharing dApp](https://github.com/mhssamadani/ErgoProfitSharingDapp): Example profit sharing contract. [`Scala`?]
*   [Trade-In Protocol](https://github.com/lucagdangelo/trade-in): Example protocol for burning and trading tokens (e.g., cards). [`Scala`, `JS/TS`]
*   [SigmaFi UI Plugins](https://github.com/capt-nemo429/sigmafi-ui/blob/main/src/offchain/plugins.ts): Example off-chain logic for SigmaFi. [`TS`]
*   [Ergo Payroll (ErgoHack)](https://github.com/andrehafner/ergo-payroll): Payroll project from ErgoHack.
*   [LETS Backend (ErgoHack)](https://github.com/arkan294/LETS-backend): Local Exchange Trading System backend from ErgoHack.
*   [Inergitance (ErgoHack)](https://github.com/inergitance): Inheritance dApp proof-of-concept from ErgoHack.
*   [dAppStep Play (ErgoPay Example)](https://github.com/nirvanush/dappstep-play): Example backend using ErgoPay signing. [`TS`]
*   [Ergo Android](https://github.com/aslesarenko/ergo-android): Example Android application demonstrating AppKit usage. [`Java`, `Kotlin`]
*   [Node Wallet Address Generation Demo (Java)](https://github.com/ergoplatform/ergo/blob/master/ergo-wallet/src/test/java/org/ergoplatform/wallet/AddressGenerationDemo.java): Example using node's internal wallet logic. [`Java`]
*   [Node Wallet Create Transaction Demo (Java)](https://github.com/ergoplatform/ergo/blob/master/ergo-wallet/src/test/java/org/ergoplatform/wallet/CreateTransactionDemo.java): Example using node's internal wallet logic. [`Java`]
*   [Ergo Asset Locker Demo](https://github.com/mowreez/ergo-asset-locker): Demo dApp locking assets. [`JS/TS`]
*   [Ergo Audit Backend Demo](https://github.com/jlsachse/ergo-audit-backend): Demo backend for auditing purposes. [`Java`]
*   [SchedulERG Demo](https://github.com/ladopixel/schedulERG): Demo using encrypted descriptions for token creation/querying. [`Python`]
*   [Ergo Offchain Demo](https://github.com/MrStahlfelge/ergo-offchain): Examples of off-chain interactions. [`Kotlin`]
*   [Fleet SDK Send NFT Demo](https://github.com/ladopixel/fleet-sdk-sendnft): Demo sending NFTs using Fleet. [`JS/TS`]
*   [Fleet SDK Create Token Demo](https://github.com/ladopixel/fleet-sdk-createtoken): Demo creating tokens using Fleet. [`JS/TS`]
*   [Fleet SDK Burn Tokens Demo](https://github.com/ladopixel/fleet-sdk-burntokens): Demo burning tokens using Fleet. [`JS/TS`]
*   [MultiSig Input Demo (WASM)](https://github.com/SavonarolaLabs/multisig-input): Example tests for signing multisig transactions with ergo-lib-wasm. [`JS`]
*   [Fleet Chained Token Sender](https://github.com/mgpai22/fleet-ergo-chained-token-sender): Demo sending tokens in chained transactions using Fleet. [`JS/TS`]
*   [AppKit by Example (ApexTheory)](https://github.com/ApexTheory/appkit-by-example): Example usage of AppKit. [`Scala`]
*   [Go Ergo Example](https://github.com/ross-weir/go-ergo-example): Example using Go with C bindings. [`Go`, `C`]
*   [Ergo Stealth Address Example](https://github.com/ross-weir/ergo-stealth-address-example): Example implementation of stealth addresses. [`JS/TS`]
*   [Ergo Playground Scenarios](https://github.com/jaysee260/ergo-playground): Collection of miscellaneous scenarios implemented on Ergo. [`Scala`?]
*   [ErgoPay Server Example](https://github.com/MrStahlfelge/ergopay-server-example): Example backend server demonstrating ErgoPay. [`Java`, `Spring`]
*   [Ergo Android Example App](https://github.com/aslesarenko/ergo-android): Example Android application demonstrating AppKit usage. [`Java`, `Kotlin`]
*   [Mosaik AgeUSD Demo](https://github.com/MrStahlfelge/mosaik-ageusddemo): Mosaik UI example for AgeUSD. [`Kotlin`?]
*   [Mosaik Tutorial Series App](https://github.com/MrStahlfelge/mosaik-tutorial-series): Example app accompanying the Mosaik tutorial. [`Kotlin`]
*   [Mosaik Token Burn Demo](https://github.com/MrStahlfelge/mosaik-demo-tokenburn): Mosaik demo UI for burning tokens with ErgoPay. [`Kotlin`]
*   [Mosaik NFT Marketplace Example](https://github.com/MrStahlfelge/mosaiknftmarketplace): Example Mosaik UI for an NFT marketplace. [`Kotlin`?]
*   [ErgoPay Frontend Example](https://github.com/MrStahlfelge/ergopay-frontend-example): Example frontend UI demonstrating ErgoPay integration. [`JS/TS`?]

## DeFi & dApps

### DEXs & Swaps

*   [Spectrum Finance](https://spectrum.fi/): Cross-chain DEX with AMM and Order Book models. [Contracts](https://github.com/spectrum-finance/ergo-dex/tree/master/contracts) | [Backend](https://github.com/spectrum-finance/spectrum-offchain-ergo) [Status: Active] [Live]
*   [DexyGold](https://dexygold.com/): Decentralized exchange platform. [Telegram](https://t.me/dexygold) | [Contracts/Spec](https://github.com/ergoplatform/ergo-jde/tree/main/kiosk/src/test/scala/kiosk/dexy) [Status: Active] [Live]
*   [GuapSwap](https://github.com/GuapSwap): Decentralized smart contract profit swapping service for miners. [Contracts](https://github.com/GuapSwap/guapswap-ronin/tree/main/src/main/scala/contracts) [Status: Active] [Live]
*   [Single Transaction Swap](https://www.single-tx-swap.com/): UI for performing atomic swaps in a single transaction. [GitHub](https://github.com/danieloravec/ergo-token-swap) [Status: Active] [Live]
*   [Arbit](https://github.com/ConnecMent/arbit): Simple arbitrage platform for Ergo (and Cardano) DEXs. [`JS`] [Status: Active?]
*   [Analog Ergo](https://github.com/dzyphr/ScalaSigmaParticle): P2P atomic swap protocol and implementation. [Contract](https://github.com/dzyphr/ScalaSigmaParticle/blob/main/ScalarLock/src/main/scala/ScalarLock.scala) | [Website/UI PoC](https://github.com/dzyphr/AtomicAnalogSwapWebsite) [Status: Active]

### Stablecoins & Lending

*   [SigmaUSD](https://sigmausd.io/): Algorithmic stablecoin protocol (AgeUSD). [EIP-15](https://github.com/ergoplatform/eips/blob/master/eip-0015.md) | [Off-chain Bot](https://github.com/anon-real/sigma-usd) | [AgeUSD Spec](https://github.com/Emurgo/age-usd) | [Telegram](https://t.me/SigmaUSD) [Status: Active] [Live]
*   [Duckpools](https://duckpools.io/): Lending platform on Ergo. [GitHub Org](https://github.com/duckpools) | [Contracts](https://github.com/duckpools/lend-protocol-contracts/tree/main/contracts) | [Option Pools](https://github.com/duckpools/off-chain-bot/tree/optionPools/optionPools) | [Telegram](https://t.me/duckpools_chat) [Status: Active] [Live]
*   [EXLE (ErgoLend)](https://ergolend.org/): Lending platform. [Contracts/Edge Lib](https://github.com/Ergo-Lend/edge) | [Telegram](https://t.me/ErgoLend) [Status: Active] [Live]
*   [SigmaFi](https://sigmafi.org/): DeFi platform offering yield strategies. [UI Repo](https://github.com/capt-nemo429/sigmafi-ui) | [Contracts Repo](https://github.com/K-Singh/Sigma-Finance) | [Telegram](https://t.me/sigmafi) [Status: Active] [Live]
*   [Phoenix Finance](https://github.com/PhoenixErgo/phoenix-hodlcoin-contracts): DeFi platform involving Hodlcoins. [Status: Active] [Live]
*   [Hodlcoin Contracts](https://github.com/lucagdangelo/hodlcoin-contracts): Contracts for the Hodlcoin concept. [Status: Active] [Live]
*   [Gluon](https://github.com/DjedAlliance): Cross-chain stablecoin infrastructure based on Djed (in development). [Twitter](https://twitter.com/DjedAlliance) [Status: In Development]

### Launchpads

*   [Ergopad](https://ergopad.io/): Decentralized launchpad for Ergo projects. [GitHub Org](https://github.com/ergopad) | [Contracts](https://github.com/ergopad/ergopad-api/tree/dev/app/contracts) | [Telegram](https://t.me/ergopad_chat) [Status: Active] [Live]

### Identity & DNS

*   [Ergonames](https://ergonames.com/): Decentralized naming service for Ergo addresses. [GitHub Org](https://github.com/ergonames) | [Contracts](https://github.com/ergonames/ergonames/tree/master/src/main/scala) | [Rust SDK](https://github.com/ergonames/sdk/tree/master/rust) [Status: Active] [Live]
*   [Bitdomains](https://bitdomains.org/): Decentralized domain name system (DNS) project. [Contracts](https://github.com/bitdomains/contracts) [Status: Paused]
*   [Ergo Reputation System](https://reputation-systems.github.io/): On-chain reputation system. [GitHub Org](https://github.com/sigma-rps) | [Library](https://github.com/reputation-systems/reputation-system-lib) | [Forum Post](https://www.ergoforum.org/t/reputation-system/4782) [Status: Active] [Beta]

### Privacy

*   [ErgoMixer](https://ergomixer.com/): Non-custodial, non-interactive mixer for ERG and tokens using Sigma protocols. [GitHub Org](https://github.com/ergoMixer/) | [Contracts/Backend](https://github.com/ergoMixer/ergoMixBack) | [Releases](https://github.com/ergoMixer/ergoMixBack/releases) [Status: Active] [Live]
*   [Sigmajoin](https://github.com/ergoplatform/ergo-jde/blob/main/kiosk/src/test/scala/kiosk/mixer/doc/main.pdf): Specification for a CoinJoin protocol using Sigma protocols. [Contracts/Tests](https://github.com/ergoplatform/ergo-jde/tree/main/kiosk/src/test/scala/kiosk/mixer) [Status: Concept/Spec]

### Gaming & Metaverse

*   [BlitzTCG](https://blitz-tcg.com/): Trading Card Game on Ergo. [Status: Active] [Beta]
*   [CyberVerse](https://cyberverseteam.itch.io/cyberverse): Metaverse/Gaming project. [Telegram](https://t.me/CyberVersegame) [Status: Active] [Live]
*   [Night Owl Casino](https://nightowlcasino.io/): Decentralized casino platform. [GitHub Org](https://github.com/nightowlcasino) [Status: Active] [Live]
*   [ObolFlip](https://github.com/ObolFlip): Decentralized CoinFlip betting application. [Client](https://github.com/ObolFlip/obolflip-client) [Status: Active?]
*   [Comet Lottery](https://github.com/mgpai22/comet-lottery): Lottery dApp contracts and bot. [`Scala`] [Status: Active?]

### DAO Frameworks

*   [Paideia](https://paideia.im/): DAO management platform and framework. [Contracts](https://github.com/paideiadao/paideia-contracts) | [Telegram](https://t.me/paideiaDAO) [Status: Active] [Beta]
*   [Ergo Team](https://github.com/anon-real/ergo-team): Simple DAO/team treasury contract example. [`ErgoScript`]

### Other dApps & Services

*   [CruxFinance](https://github.com/cruxfinance): Cross-chain liquidity solutions and tools. [`Scala`, `Rust`, `JS/TS`] [Status: Active] [Live]
*   [Machina Finance](https://github.com/nautls/machina-finance): Framework and platform for off-chain execution bots (Ergomatic). [`JS/TS`] [Status: Active]
*   [thz.fm](https://thz.fm/): Decentralized media/music platform. [Contracts](https://github.com/TremendouslyHighFrequency/SmartContracts) | [Telegram](https://t.me/swampoflife) [Status: Active] [Beta]
*   [Hodlbox](https://hodlbox.xyz/): Create time-locked boxes for tokens. [GitHub](https://github.com/SavonarolaLabs/hodlbox-xyz) | [Contracts](https://github.com/SavonarolaLabs/hodlbox-xyz/tree/main/src/lib/contract) [Status: Active] [Live]
*   [SigmaO](https://sigmao.cc/): Options trading platform. [GitHub](https://github.com/ThierryM1212/sigmao) | [Telegram](https://t.me/SigmaOpts) [Status: Active] [Beta]
*   [Netnotes](https://github.com/networkspore/Netnotes-Linux/releases): Secure P2P messaging/notes application. [`Java`] [Status: Active] [Beta]
*   [TabbyPOS](https://tabbypos.com/): Point-of-Sale system utilizing Ergo. [GitHub](https://github.com/Kolmen-Tech/ErgoPOS) | [Telegram](https://t.me/tabbypos) [Status: Active] [Live]
*   [Azorus](https://azorus.io/): Toolkit/platform for interacting with Ergo. [GitHub](https://github.com/gsblabsio/azorus) | [Telegram](https://t.me/azorus_xyz) [Status: Paused]
*   [SigmaStamp](https://www.sigmastamp.ml/): Notary/timestamping service. [GitHub](https://github.com/sigmastamp) [`JS/TS`] [Status: Paused]
*   [Benefaction Platform](https://github.com/StabilityNexus/BenefactionPlatform-Ergo): Charity/Donation platform prototype. [Status: Development]
*   [Moria Finance](https://github.com/Moria-Finance): DeFi project focusing on ERG derivatives (in development). [Status: Development]
*   [ChainCash](https://github.com/ChainCashLabs): Decentralized monetary system combining trust and blockchain assets. [Whitepaper](https://github.com/kushti/chaincash/blob/master/paper/chaincash.pdf) | [Rust Server](https://github.com/ChainCashLabs/chaincash-rs) | [Contracts](https://github.com/ChainCashLabs/chaincash/tree/master/contracts) [Status: Active]
*   [Sigma Subscriptions](https://github.com/cornbelt-dev/sigma-subscriptions): Framework for running subscription services on Ergo. [Status: Paused?]
*   [ErgoWell](https://github.com/mhssamadani/ErgoWell): Concept for a crowdfunding/venture investment platform. [`JS/TS`] [Status: Development]
*   [Lithos Protocol](https://lithosprotocol.org/): DeFi protocol aiming to bring liquidity to ERG. [GitHub Org](https://github.com/Lithos-Protocol) | [LitePaper](https://github.com/Lithos-Protocol/LitePaper) [Status: Active]
*   [Off The Grid](https://github.com/Telefragged/off-the-grid): Decentralized grid trading bot. [`Rust`]
*   [Sigmarand](https://github.com/noob77777/ergo-randgen): Commit-Reveal Random Number Generation scheme. [`Scala`]
*   [Community Liquidity Bootstrap](https://github.com/AcoSmrkas/community-liquidity-bootstrap): Platform for community liquidity bootstrapping (ErgoHack VII). [`JS/TS`?]
*   [Perma Ergo](https://github.com/firashebili/permergo-microfinancing-dao): RealFi micro-finance project for farmers (ErgoHack VI).
*   [DumDumDum](https://github.com/kii-dot/dumdumdum): Decentralised, on-chain Twitter alternative using NFTs (ErgoHack V). [`Scala`?]

## NFT Ecosystem

### Marketplaces & Auctions

*   [SkyHarbor](https://skyharbor.io/): NFT marketplace. [Contracts](https://github.com/skyharbor-market/contracts) [Status: Active] [Live]
*   [AuctionHouse](https://ergoauctions.org/): NFT auction platform based on EIP-22. [GitHub](https://github.com/anon-real/ErgoAuctionHouse) | [EIP-22](https://github.com/ergoplatform/eips/blob/master/eip-0022.md) | [Telegram](https://t.me/ergoauctionhouse) [Status: Active] [Live]

### Minting & Utilities

*   [Lilium](https://lilium.digital/): NFT tools, minting, and services. [GitHub Org](https://github.com/LiliumErgo) | [Contracts](https://github.com/LiliumErgo/scala-api/blob/main/app/contracts/LiliumContracts.scala) [`Scala`, `JS/TS`, `Python`] [Status: Active] [Live]
*   [ErgoRaffle](https://ergoraffle.com/): Decentralized raffle platform often used for NFTs. [GitHub](https://github.com/ErgoRaffle) | [Contracts](https://github.com/ErgoRaffle/raffle-backend/blob/master/app/raffle/RaffleContract.scala) [Status: Active] [Live]
*   [Ergo NFT Bulk Minter](https://github.com/mgpai22/ergo-nft-bulk-minter): Python script for bulk minting NFTs (includes royalty support). [`Python`]
*   [Ergo Token Minter](https://thierrym1212.github.io/tokenminter/): Web UI for minting tokens/NFTs. [GitHub](https://github.com/ThierryM1212/ergo-token-minter) [`JS/TS`]
*   [CYTI](https://thierrym1212.github.io/cyti/): Choose Your Token ID - Minable contract for minting tokens with specific ID prefixes. [GitHub](https://github.com/ThierryM1212/cyti) [`JS/TS`]
*   [Sigma Mint](https://github.com/thedlop/sigma_mint): Ruby library for NFT minting (ErgoHack IV). [`Ruby`]

### NFT Projects

*   [Auction Coin](https://auctioncoin.app/): Platform related to auctions, using NFTs. [GitHub Org](https://github.com/orgs/Auction-Coin/repositories) | [Contracts](https://github.com/Auction-Coin/contracts) [Status: Active] [Deployed Contract]
*   [Blobstopia](https://github.com/ThierryM1212/blobs-topia/): Completed generative NFT project/game. [Release](https://github.com/ThierryM1212/blobs-topia/releases/tag/v1.1.0) [Status: Done]

## Mining

### Pools

*   [GetBlok.io Pool](https://ergo.getblok.io/): Popular Ergo mining pool.
*   [MiningCore](https://github.com/oliverw/miningcore): Open-source mining pool software supporting Ergo. [Config Wiki](https://github.com/oliverw/miningcore/wiki/Configuration)
*   [NOMP (ergo-nomp)](https://github.com/btclinux/ergo-nomp): Node Open Mining Portal adapted for Ergo.
*   [Node Stratum Pool](https://github.com/vorujack/node-stratum-pool): Node.js based stratum pool server. [`JS`]
*   [ergo-mining-pool (MGpai)](https://github.com/mgpai22/ergo-mining-pool): Open source mining pool. [`Go`?]

### Software

*   [Autolykos2 Nvidia Miner](https://github.com/mhssamadani/Autolykos2_NV_Miner): Open-source Nvidia GPU miner for Autolykos2.
*   [Autolykos2 AMD Miner](https://github.com/mhssamadani/Autolykos2_AMD_Miner): Open-source AMD GPU miner for Autolykos2.
*   [Autolykos2 CPU Miner](https://github.com/mhssamadani/Autolykos2-CPUMiner): Open-source CPU miner for Autolykos2.
*   [Autolykos GPU Miner (v1)](https://github.com/ergoplatform/Autolykos-GPU-miner): Original open-source GPU miner (Autolykos v1).
*   [Ergo AMD Miner (v1)](https://github.com/mhssamadani/ergoAMDminer): Open-source AMD miner (Autolykos v1).
*   *Note: Several closed-source miners exist (lolMiner, Nanominer, SRBMiner, NBMiner, TeamRedMiner, T-Rex), see [Mining Software Comparison](mining/software.md) for links and fee info.*

### Utilities & Tooling

*   [ErgoStratumServer](https://github.com/mhssamadani/ErgoStratumServer): Stratum server implementation. [`Scala`] | [Reqlez Fork](https://github.com/reqlez/ErgoStratumServer)
*   [ErgoStratumProxy](https://github.com/mhssamadani/ErgoStratumProxy): Stratum proxy for connecting open-source miners. [`Scala`]
*   [Stratum4Ergo](https://github.com/Satergo/stratum4ergo): Java library for creating Stratum mining pool servers. [`Java`]
*   [Ergo Profit Calculator](https://babygrenade.github.io/ergo-profit-calc/): Web-based mining profitability calculator.
*   [ErgoTools (Mining Rewards)](https://github.com/lorien/ergotools): CLI tool to find and withdraw miner rewards.
*   [Miner Rewarder](https://github.com/mgpai22/miner-rewarder): Bot to reward miners based on specific criteria. [`JS/TS`]
*   [Miner Reward Consolidator](https://github.com/mgpai22/ergo-miner-reward-consolidator): Tool to consolidate mining rewards. [`JS/TS`?]
*   [Miner Rights Protocol](https://github.com/The-Last-Byte-Bar/Miner-Rights-Protocol): Concept/protocol for rights-based mining token distribution.
    *   [Token Flight](https://github.com/The-Last-Byte-Bar/Token-Flight): Implementation related to Miner Rights Protocol.
    *   [Token Flight Bot](https://github.com/The-Last-Byte-Bar/Token-Flight-Bot): Bot for Token Flight.

### Smart Pooling

*   [ErgoSmartPools](https://github.com/WilfordGrimley/ErgoSmartPools): Decentralized mining pool using smart contracts.
*   [GetBlok Subpooling Contracts](https://github.com/GetBlok-io/ergo-smartpooling-contracts): Smart contracts used in GetBlok's subpooling system. [`Scala`]
*   [GetBlok Subpooling Plasma Configs](https://github.com/GetBlok-io/Subpooling/tree/mainnet_plasma/conf/scripts): Scripts related to GetBlok's Plasma implementation for subpooling.

## Standards (EIPs)

*   [EIP Repository](https://github.com/ergoplatform/eips): Official repository for Ergo Improvement Proposals.
*   [EIP-1: Ergo Address Types](https://github.com/ergoplatform/eips/blob/master/eip-0001.md)
*   [EIP-3: HD Wallet Derivation Paths](https://github.com/ergoplatform/eips/blob/master/eip-0003.md)
*   [EIP-4: Asset Standard (Tokens & NFTs)](https://github.com/ergoplatform/eips/blob/master/eip-0004.md)
*   [EIP-5: ErgoScript Templates (Deprecated)](https://github.com/ergoplatform/eips/blob/master/eip-0005.md)
*   [EIP-6: Headless dApp Protocol](https://github.com/ergoplatform/eips/blob/master/eip-0006.md)
*   [EIP-11: Asset Issuance Box Standard](https://github.com/ergoplatform/eips/pull/11)
*   [EIP-12: dApp Connector Interface](https://github.com/ergoplatform/eips/pull/23/files)
*   [EIP-15: SigmaUSD Protocol](https://github.com/ergoplatform/eips/blob/master/eip-0015.md)
*   [EIP-16: Oracle Pool V2 (Draft)](https://github.com/ergoplatform/eips/blob/eip16/eip-0016.md)
*   [EIP-17: Proxy Contracts Standard](https://github.com/ergoplatform/eips/blob/master/eip-0017.md)
*   [EIP-19: Cold Wallet Standard](https://github.com/ergoplatform/eips/blob/master/eip-0019.md)
*   [EIP-20: ErgoPay URI Scheme](https://github.com/ergoplatform/eips/blob/master/eip-0020.md)
*   [EIP-21: URI Scheme for Token Payments](https://raw.githubusercontent.com/ergoplatform/eips/master/eip-0021.md) (Draft)
*   [EIP-22: Auction Contract Standard](https://github.com/ergoplatform/eips/blob/master/eip-0022.md)
*   [EIP-23: Oracle Pool V2 Bootstrap Standard](https://github.com/ergoplatform/eips/tree/cae50b722d6929c794847d21668500acb01f3c8c/eip-0023/contracts)
*   [EIP-24: Digital Artwork / NFT Standard](https://github.com/ergoplatform/eips/blob/master/eip-0024.md)
*   [EIP-25: Payment Request URI Scheme](https://github.com/ergoplatform/eips/blob/master/eip-0025.md)
*   [EIP-27: Miner Voting Parameters](https://github.com/ergoplatform/eips/blob/master/eip-0027.md)
*   [EIP-31: Babel Fees Standard](https://github.com/ergoplatform/eips/blob/master/eip-0031.md)
*   [EIP-33: Crowdfunding Contract Standard](https://github.com/ergoplatform/eips/pull/33)
*   [EIP-37: Autolykos v2 Update](https://github.com/ergoplatform/eips/blob/ddbca24fef5e91e0c80c6881fc31d8831ae69768/eip-0037.md)
*   [EIP-38: Partial Voting for Miners (Draft)](https://github.com/WilfordGrimley/eip38PartialVoting)
*   [EIP-39: Just-In-Time Costing (JITC)](https://github.com/ergoplatform/eips/blob/master/eip-0039.md)
*   [EIP-41: Stealth Addresses (Draft)](https://raw.githubusercontent.com/ergoplatform/eips/d21280977f2c21dc733632c48c98d0f614bc6123/eip-0041.md)
*   [EIP-43: Reduced Transaction](https://github.com/ergoplatform/eips/pull/91)
*   [EIP-44: Arbitrary Data Signing](https://github.com/ergoplatform/eips/pull/92)
*   [EIP-45: Storage Rent Redistribution (Draft)](https://github.com/ergoplatform/eips/pull/93)
*   [EIP-46: Authentication Message Signing (Draft)](https://github.com/ergoplatform/eips/blob/2de4ea0deff12a276f74df57ef3a14dab2c5dfb8/eip-0046.md)
*   [EIP-47: Re-emission Contract Standard (Draft)](https://github.com/ergoplatform/eips/blob/0836dd1eca323c6b5fd6b5172c27a465bd4449cd/eip-0047.md)
*   [EIP-50: Context Extension Clarification (Draft)](https://github.com/ergoplatform/eips/blob/a24fc414abbc10e6ee59f878b280d9ecc725e10c/eip-0050.md)
*   [SigmaUSD Improvement Proposals (SIPs)](https://github.com/ergoplatform/sips): Repository for proposals related to the SigmaUSD protocol.

## Explorers & Dashboards

*   [Ergo Explorer (Official)](https://explorer.ergoplatform.com/): The primary Ergo blockchain explorer. [Frontend](https://github.com/ergoplatform/explorer-frontend) | [Backend](https://github.com/ergoplatform/explorer-backend)
*   [Sigmaspace](https://sigmaspace.io/): Alternative explorer with additional tools and charts.
*   [ErgoWatch](https://ergo.watch/): Network statistics, tokenomics, and analytics dashboard. [GitHub](https://github.com/abchrisxyz/ergowatch)
*   [erg-explorer](https://github.com/AcoSmrkas/ErgExplorer): Community-built alternative explorer. [`JS/TS`] [Telegram](https://t.me/ErgExplorer)
*   [uexplorer](https://github.com/pragmaxim/ergo-uexplorer): Minimalist explorer focused on UTXO set browsing. [`Scala`]
*   [Indexed Node Explorer](https://github.com/Luivatra/indexed-node-explorer): Simple explorer UI for an indexed Ergo node. [`JS/TS`]
*   [Ergo Nodes Dashboard](http://ergonodes.net/): Network map and node statistics dashboard. [GitHub](https://github.com/Satergo/Ergonnection)
*   [Paizo Mining Vote Simulator](https://deadit.github.io/paizo/): Tool for simulating miner voting based on EIP-27. [GitHub](https://github.com/deadit/paizo)
*   [ErgCube](https://ergcube.com/): Community dashboard and information site.
*   [Testnet Explorer](https://testnet.ergoplatform.com/): Explorer for the Ergo test network.
*   [Testnet Faucet](https://testnet.ergofaucet.org/): Faucet for obtaining testnet ERG.

## Analytics

*   [ErgoVision](https://github.com/CryptoCream/ErgoVision): Wallet visualization tool for investigating transactions and addresses. [`Python`]
    *   [ErgoVision Colab Notebook](https://colab.research.google.com/drive/13O_6XEHi7xbjuhzby0s7YGX0rshrClXK?usp=sharing): Google Colab version.
*   [SigmaUSD Bank Analysis Notebook](https://colab.research.google.com/drive/1iA_PPvWrJGjdpOFYME7W_lQrU4BemaE4?usp=sharing): Google Colab notebook for analyzing SigmaUSD bank transactions. [`Python`]
*   [ergo-intelligence](https://github.com/Eeysirhc/ergo-intelligence): Tools, guides, and resources for blockchain analysts.
*   [tidyergo](https://github.com/Eeysirhc/tidyergo): R/Tidyverse package for Ergo blockchain statistics. [`R`]
*   [ergo-analytics](https://github.com/gsblabsio/ergo-analytics): Docker setup for extracting insights from the Ergo network. [`Docker`]
*   [ErgoStats Android](https://github.com/sachindayl/ErgoStatsAndroid): Android app for Ergo network stats. [`Kotlin`/`Java`]
*   [ErgoStats iOS](https://github.com/ach2swift/ErgoStats): iOS app for Ergo network stats. [`Swift`]
*   [Ergo Tokenautics](https://github.com/babygrenade/ergo-tokenautics): Token distribution analysis/tool. [`Python`]
*   [Ergo Token Analysis (Freebyo)](https://github.com/freeboy0/ergo-token-analysis): Token analysis tools. [`Python`?]
*   [Developer Activity (Artemis)](https://app.artemis.xyz/developer-activity?ecosystemValue=Ergo): Tracks developer activity based on GitHub commits.
*   [Developer Activity (DeveloperReport)](https://www.developerreport.com/ecosystems/ergo): Alternative view of developer activity.
*   [Ergo Node Metrics Report Notebook](https://github.com/ergoplatform/ergo/blob/master/metrics/Report.ipynb): Jupyter notebook for analyzing node performance metrics. [`Python`]

## Community & Resources

### Information Hubs

*   [Ergo Platform Website](https://ergoplatform.org/): Official website with news, overview, and ecosystem links. [GitHub](https://github.com/ergoplatform/website)
*   [Ergo Documentation](https://docs.ergoplatform.com/): Official documentation for users, developers, and miners. [GitHub](https://github.com/ergoplatform/ergodocs)
*   [Ergonaut Handbook](https://ergonaut.space/): Community-driven wiki and handbook.
*   [Sigmaverse](https://sigmaverse.io/): Directory of dApps and tools in the Ergo ecosystem. [GitHub](https://github.com/ergoplatform/sigmaverse)
*   [ErgoForum](https://www.ergoforum.org/): Official community discussion forum.
*   [Ergo Discord](https://discord.gg/ergo-platform-668903786361651200): Main community chat server. *(Note: Verify invite link is current)*
*   [Ergo Telegram](https://t.me/ergoplatform): Main Telegram group.
*   [Ergo Reddit](https://www.reddit.com/r/ergonauts/): Subreddit for Ergo discussion.
*   [Awesome Ergo](https://github.com/ergoplatform/awesome-ergo): This curated list of resources.
*   [Ergo Sites](https://ergosites.github.io/): Community-maintained list of Ergo-related websites.
*   [Ergo Platform Wiki](https://github.com/ergoplatform/ergo/wiki): Official GitHub wiki for the node software.
*   [Ergo Foundation Website](https://ergofoundation.org/): Information about the Ergo Foundation.
*   [Ergo Platform GitHub Discussions](https://github.com/ergoplatform/ergo/discussions): Forum for discussing node development and technical topics.

### Contribution Platforms

*   [Ergo Bounties](https://github.com/ErgoDevs/Ergo-Bounties): Platform for finding and funding development bounties.
*   [Grow Ergo Issues](https://github.com/ergoplatform/grow-ergo/issues): GitHub issues tracking ecosystem growth tasks and proposals.
*   [Ergo Node Issues](https://github.com/ergoplatform/ergo/issues): Main issue tracker for the reference node software.
*   [Analytics Ecosystem Data](https://github.com/electric-capital/crypto-ecosystems/blob/master/data/ecosystems/e/ergo.toml): Add your project here to be tracked by developer activity sites.

### Education & Tutorials

*   [DeCo Education](https://deco-education.github.io/deco-docs/docs/intro): Educational platform with courses on Ergo.
    *   [Into the Woods Course](https://deco-education.github.io/deco-docs/docs/category/into-the-woods): Introductory course.
    *   [ErgoScript Developer Course](https://github.com/DeCo-Education/ErgoScript-Developer-Course): More advanced ErgoScript course.
*   [Zack Balbin's Ergo Tutorials](https://github.com/zackbalbin/ErgoTutorials): Collection of Scala tutorials for Ergo. [`Scala`]
*   [Ergo Community YouTube](https://www.youtube.com/@ErgoPlatform): Official YouTube channel with AMAs, tutorials, presentations.
*   [ErgoFoundation YouTube](https://www.youtube.com/@ErgoFoundation): Foundation-focused YouTube channel.
*   [Using Appkit from Python (Wiki)](https://github.com/ergoplatform/ergo-appkit/wiki/Using-Appkit-from-Python): Guide for using AppKit with Python via JPype.
*   [Ergo Full Node on Raspberry Pi Guide](https://github.com/ccgarant/ergo-full-node-raspi): Community guide for setting up a full node on a Raspberry Pi.
*   [Fleet SDK Documentation](https://fleet-sdk.github.io/docs/): Official documentation for the Fleet SDK.
    *   [Fleet Compiler Docs](https://fleet-sdk.github.io/docs/compiler)
    *   [Fleet Serializer Overview](https://fleet-sdk.github.io/docs/serializer-overview)
    *   [Fleet Babel Fees Plugin Docs](https://fleet-sdk.github.io/docs/plugins/babel-fees)

### Papers & Specifications

*   [Ergo Whitepaper](https://ergoplatform.org/en/documents/): The foundational document outlining Ergo's design and principles.
*   [ErgoScript Whitepaper](https://ergoplatform.org/docs/ErgoScript.pdf): Detailed paper on the ErgoScript language.
*   [Autolykos PoW Algorithm](https://ergoplatform.org/docs/ErgoPow.pdf): Paper describing the Autolykos proof-of-work algorithm.
*   [NiPoPoWs Paper](https://eprint.iacr.org/2016/994.pdf): Research paper on Non-Interactive Proofs of Proof-of-Work.
*   [Storage Rent Paper](https://ergoplatform.org/docs/StorageRent.pdf): Paper detailing the storage rent mechanism.
*   [Sigma Protocols Paper](https://ergoplatform.org/docs/ergoscript.pdf): (ErgoScript Whitepaper also covers Sigma protocols in detail).
*   [ErgoTree Specification](https://raw.githubusercontent.com/ScorexFoundation/sigmastate-interpreter/master/docs/spec/ergotree.pdf): Formal specification of the ErgoTree serialization format.
*   [ErgoScript Language Specification](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/LangSpec.md): Specification of the ErgoScript language syntax and semantics.
*   [Sigma Language DSL Documentation](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/sigma-dsl.md): Documentation for the Sigma-protocol based language features.
*   [Know Your Assumptions (KYA)](https://github.com/kushti/kya): Framework for analyzing assumptions in blockchain protocols. [PDF](https://github.com/kushti/kya/blob/master/kya.pdf)
*   [ChainCash Whitepaper](https://github.com/kushti/chaincash/blob/master/paper/chaincash.pdf): Paper describing the ChainCash protocol.
    *   [ChainCash Server Docs](https://github.com/ChainCashLabs/chaincash/blob/master/docs/server.md): Documentation for the ChainCash server implementation.
*   [High Level Design Patterns In Extended UTXO Systems](https://github.com/Emurgo/Emurgo-Research/blob/master/smart-contracts/High%20Level%20Design%20Patterns%20In%20Extended%20UTXO%20Systems.md): Research on dApp patterns in eUTXO systems.
*   [Ergo Scala Style Guide](https://github.com/ergoplatform/ergo-scala-style-guide): Style guide for contributing Scala code to Ergo projects.
*   [Ergo Social Contract](https://ergoplatform.org/en/blog/2022-04-26-the-ergo-manifesto-revised-edition/): The guiding principles and manifesto of the Ergo Platform.
*   [On Contractual Money](https://ergoplatform.org/docs/AdvancedErgoFeatures.pdf): Paper discussing advanced features and the concept of contractual money in Ergo.
*   [ErgoScript Compiler Documentation](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/ergoscript-compiler.md): Details on the ErgoScript compiler internals.
*   [ErgoScript Performance & Style Guide](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/perf-style-guide.md): Tips for writing efficient ErgoScript.
*   [Ergo Platform Improvement Proposals (EIPs)](https://github.com/ergoplatform/eips): Repository for all EIPs.
*   [SLIP-0044 : Registered coin types for BIP-0044](https://github.com/satoshilabs/slips/blob/master/slip-0044.md): Ergo is registered with coin type `429`.
*   [Ergo Subblocks Paper](https://raw.githubusercontent.com/ergoplatform/ergo/e15dcd0b4ca0a72d32d97228f010d813540de39d/papers/subblocks/subblocks.md): Research paper on the sub-block concept for sidechains/scalability.
*   [Ergohack Sidechain Whitepaper](https://github.com/ross-weir/ergohack-sidechain/blob/main/docs/whitepaper/sidechain.pdf): Whitepaper for the Ergohack sidechain proof-of-concept.
*   [Ergohack Sidechain Repo](https://github.com/ross-weir/ergohack-sidechain): Ergohack sidechain proof-of-concept repo. [`Rust`?]
*   [Stealth Address Docs (Aragogi)](https://github.com/aragogi/Stealth-doc): Documentation for a stealth address scanner/mixer concept.

### Utilities

*   [ErgoTipper Token List](https://github.com/Luivatra/ergotipper-tokens): Repository defining tokens recognized by the ErgoTipper bot on Discord/Telegram.
*   [Spectrum Token List](https://github.com/spectrum-finance/ergo-token-list): Token list curated by the Spectrum Finance team.
*   [ErgoToolsBot (Telegram)](https://t.me/ergotoolsbot): Telegram bot providing various Ergo utilities. [GitHub](https://github.com/ladopixel/ErgoToolsBot) [`Python`]
*   [Matterbridge](https://github.com/42wim/matterbridge): Software used for bridging Ergo community chats between Discord and Telegram.
*   [SharkNet](https://github.com/The-Last-Byte-Bar/SharkNet): Community-curated dataset of ErgoScript examples for training AI/ML models for developer tooling.
