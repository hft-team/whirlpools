# Orca Whirlpools SDKs

![Overview of Orca Whirlpools SDK suite](/../whirlpools/img/01-Welcome/orca-sdks-overview-rustdocs.png)

The Whirlpools SDKs are Orca's primary set of SDKs designed to provide enhanced, modular interaction with the Whirlpool Program on Solana and Eclipse. Whether you are managing liquidity, building applications that require pool infrastructure, or building automation tools that interact with the program, our SDKs cover a spectrum of functionality from low-level granular control to high-level abstractions. This offering is divided into three main components:

### 1. High-Level SDK (in development, requires Solana SDK v1.18)
The High-Level SDK is our top recommendation for anyone who wants to integrate with the Whirlpool Program. It builds upon the Low-Level and Core SDKs to provide an easy-to-use interface for interacting with the Whirlpool Program. This SDK abstracts many of the underlying complexities, such as tick array management, and makes managing pools and positions, and executing swaps much simpler. It is suitable for developers who need efficient, high-level functionalities and want to minimize manual configuration and management.

### 2. Core SDK
The Core SDK provides essential utilities for math operations and quotes, required for working with liquidity pools. This library focuses on calculations such as determining position status, price conversions, and computing quotes on adjusting liquidity and swaps. It is written in Rust but has been compiled to WebAssembly (Wasm) for easy integration into TypeScript projects.

### 3. Low-Level SDK (requires Solana SDK \<v2)
The Low-Level SDK is autogenerated from the Whirlpool Program's Interface Description Language (IDL). This SDK provides direct program interactions and is designed for developers who need complete, low-level control over Whirlpool operations. It covers direct access to Solana accounts, instructions, and transactions.