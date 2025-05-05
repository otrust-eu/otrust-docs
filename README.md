# OTRUST Documentation

Documentation for the OTRUST distributed truth protocol.

## What is OTRUST?

OTRUST is an innovative distributed verification system that combines cryptographic verification, semantic structuring, and lightweight blockchain technology to create a decentralized fact-checking ecosystem. The system lets users create, confirm and assess claims in a decentralized network where trust is built organically through cryptographically verified interactions.

## Documentation Index

The OTRUST documentation is organized into the following sections:

### Overview
- [OTRUST Overview](OTRUST-Overview.md) - A high-level introduction to the OTRUST protocol and ecosystem

### User Documentation
- [OTRUST User Guide](OTRUST-User-Guide.md) - A comprehensive guide for end users
- [OTRUST CLI Guide](OTRUST-CLI-Guide.md) - Documentation for the Command Line Interface

### Developer Documentation
- [OTRUST API Reference](OTRUST-API-Reference.md) - Complete API documentation
- [OTRUST Integration Guide](OTRUST-Integration-Guide.md) - How to integrate OTRUST with other systems

### Deployment Documentation
- [OTRUST Deployment Guide](OTRUST-Deployment-Guide.md) - How to deploy the OTRUST server
- [OTRUST Database Configuration Guide](OTRUST-Database-Configuration-Guide.md) - Database setup and maintenance

## OTRUST Repositories

The OTRUST ecosystem consists of three main repositories:

- [otrust-server](https://github.com/otrust-eu/otrust-server) - Server implementation with API and blockchain
- [otrust-cli](https://github.com/otrust-eu/otrust-cli) - Command-line interface for interacting with the server
- [otrust-docs](https://github.com/otrust-eu/otrust-docs) - Documentation (this repository)

## Quick Start

To get started with OTRUST:

1. **Set up the server**:
   ```bash
   git clone https://github.com/otrust-eu/otrust-server.git
   cd otrust-server
   npm install
   cp .env.example .env
   # Edit .env as needed
   npm start
   ```

2. **Install the CLI**:
   ```bash
   npm install -g otrust-cli
   otrust-cli config --server http://localhost:3000
   otrust-cli init
   otrust-cli register
   ```

3. **Create your first claim**:
   ```bash
   otrust-cli claim:create --interactive
   ```

For more detailed instructions, see the [OTRUST User Guide](OTRUST-User-Guide.md).

## Features

- **Cryptographically Verified Claims**: All claims are digitally signed by their creator
- **Semantic Structure**: Claims follow subject-predicate-object format for machine readability
- **Lightweight Blockchain**: Immutability without the performance cost of traditional blockchains
- **Distributed Reputation System**: Users build trust based on the quality of their contributions
- **Proof Chains**: Support for verification, disputation, or invalidation of claims
- **Node Federation**: Synchronization between OTRUST nodes

## Contributing

We welcome contributions to the OTRUST documentation. Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

This documentation is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
