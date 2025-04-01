# Blit Labs Documentation

Blit Labs maintains a **modular repository structure** to support **Parity Protocol**, a **distributed, verifiable, cloudless compute execution network**. Below is an overview of our repositories, setup instructions, and contribution guidelines.

---
## Repository Overview

### Architecture
For a detailed architecture of Parity Protocol, visit our [Notion Brain](https://blitlabs.com/docs).

### Core Repositories
Blit Labs manages the following key repositories:

#### [parity-runner](https://github.com/theblitlabs/parity-runner)
- Executes computational tasks in a **secure, isolated environment** (Docker or similar).
- Reports execution results and system usage metrics for validation and rewards.
- Ensures task integrity and efficient resource utilization.

#### [parity-server](https://github.com/theblitlabs/parity-server)
- Core backend handling **task distribution, validation, and reward allocation**.
- Manages **runner registration, reputation tracking, and task verification**.
- Implements **webhook-based real-time communication** with runners.

#### [parity-client](https://github.com/theblitlabs/parity-client)
- **User interface** for submitting and monitoring compute tasks.
- Provides **APIs for task management, execution tracking, and analytics**.

---
## Supporting Repositories
These repositories provide essential utilities for Blit Labs services:

- **[gologger](https://github.com/theblitlabs/gologger)**: Lightweight, structured logging library for Go, used across services for efficient debugging and monitoring.
- **[deviceid](https://github.com/theblitlabs/deviceid)**: Unique device identification system to ensure secure authentication and runner verification.
- **[keystore](https://github.com/theblitlabs/keystore)**: Secure storage solution for managing cryptographic keys and sensitive data.
- **[go-wallet-sdk](https://github.com/theblitlabs/go-wallet-sdk)**: Go-based SDK for blockchain wallet interactions, enabling **seamless on-chain reward distribution**.

---
## Setup Guide

Follow these steps to set up and run the system:

### 1. Authentication Setup
Run the following command in the **runner** or **client** repository to authenticate:
```sh
go run cmd/main.go auth --private-key <PRIVATE_KEY>
```

### 2. Start Parity Server
Run the following command in the **[parity-server](https://github.com/theblitlabs/parity-server)** repository:
```sh
make run
```

### 3. Stake Tokens
Run the following command in the **runner** or **client** repository to stake tokens:
```sh
go run cmd/main.go stake --amount 10
```

### 4. Start Parity Client
Run the following command in the **[parity-client](https://github.com/theblitlabs/parity-client)** repository:
```sh
make run
```

### 5. Start Parity Runner
Run the following command in the **[parity-runner](https://github.com/theblitlabs/parity-runner)** repository:
```sh
make run
```

---
## Contribution Guide

We welcome contributions! Follow these guidelines to get started:

- Each repository has its own **contribution and issue-tracking workflow**.
- Refer to the respective **README** files for setup instructions and coding standards.
- Submit **pull requests (PRs)** with clear descriptions and adhere to best practices.
- Join discussions and stay updated through GitHub issues.

For any questions, open an issue in the relevant repository.

