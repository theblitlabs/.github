# Blit Labs  

Blit Labs maintains a modular repository structure to support **Parity Protocol**, a Distributed—verifiable—cloudless—compute execution network. Below is an overview of our repositories and their roles.  

## Repository Overview  
Blit Labs manages the following key repositories:  

1. **[parity-runner](https://github.com/theblitlabs/parity-runner)**  
   - The execution node responsible for running computational tasks.  
   - Fetches and executes tasks using Docker or other sandboxed environments.  
   - Reports results and system usage metrics for validation and rewards.  

2. **[parity-server](https://github.com/theblitlabs/parity-server)**  
   - The core backend responsible for task distribution, validation, and reward allocation.  
   - Manages runner registration, reputation tracking, and task verification.  
   - Implements a webhook connection mechanism for real-time communication with runners.  

3. **[parity-client](https://github.com/theblitlabs/parity-client)**  
   - A user-facing interface for task submission and execution tracking.  
   - Provides APIs for managing tasks and monitoring progress.  

## Supporting Repositories  

- **[gologger](https://github.com/theblitlabs/gologger)**: A lightweight, structured logging library for Go, used across Blit Labs services for efficient debugging and monitoring.  
- **[deviceid](https://github.com/theblitlabs/deviceid)**: A unique device identification system to ensure secure authentication and runner verification.  
- **[keystore](https://github.com/theblitlabs/keystore)**: A secure storage solution for managing cryptographic keys and sensitive data.  
- **[go-wallet-sdk](https://github.com/theblitlabs/go-wallet-sdk)**: A Go-based SDK for interacting with blockchain wallets, facilitating seamless on-chain reward distribution.  

## Contribution Guide  
- Each repository follows its own contribution and issue-tracking workflow.  
- Please refer to the respective README files for setup instructions and coding guidelines.  
