---
title: Add new Contract
---

Clarinet can handle adding a new contract and its configuration to your project when you use the command listed below.

```bash
$ clarinet contract new bbtc
```

Clarinet will add two files to your project:
- the contract file in the `contracts` directory
- the contract test file in the `tests` directory

```bash
.
├── Clarinet.toml
├── contracts
│   └── bbtc.clar
├── settings
│   └── Devnet.toml
│   └── Mainnet.toml
│   └── Testnet.toml
└── tests
    └── bbtc_test.ts
```

Clarinet will also add your contract configuration in the `Clarinet.toml`.

```toml
[contracts.my-contract]
path = "contracts/my-contract.clar"
```

You can add contracts to your project by adding the files manually; however, you must make sure to add the appropriate configuration
to `Clarinet.toml` for Clarinet to recognize the contracts.

