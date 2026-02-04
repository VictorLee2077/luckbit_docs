# Luckbit Wallet Privacy Policy

Languages: [简体中文](privacy-policy.html) | English | [繁體中文](privacy-policy.zh-TW.html) | [日本語](privacy-policy.ja.html) | [한국어](privacy-policy.ko.html) | [Français](privacy-policy.fr.html) | [Español](privacy-policy.es.html) | [Русский](privacy-policy.ru.html) | [العربية](privacy-policy.ar.html)

Last updated: 2026-02-05

This Privacy Policy applies to the Luckbit Wallet browser extension ("the Extension"). The Extension is a non-custodial wallet. Private keys are encrypted and stored locally. We do not custody or access your private keys or assets.

## 1. Information We Collect
We **do not collect, store, or sell** any personally identifiable information.  
No account or login is required to use core features.

## 2. Local Data Storage
To provide wallet functionality, the Extension stores the following data **locally on your device** (not uploaded):
- Encrypted private keys / seed phrases
- Account and network configuration
- Token information and transaction cache
- User settings (language, auto-lock, etc.)

All sensitive data is encrypted locally. The Extension cannot read your private keys or seed phrases in plaintext.

## 3. Communication with Third Parties
To query blockchain data or broadcast transactions, the Extension communicates with blockchain nodes and block explorers. These requests may include:
- Wallet addresses
- Transaction hashes
- Network and chain IDs
- Your device IP address (as part of normal network requests)

This communication is only for providing wallet functionality. We **do not** share or sell your data to third parties.

## 4. Permission Disclosure (Privacy-Related)

The Extension requests the following browser permissions to provide wallet functionality. We promise **not to collect your browsing history or website data**.

### storage / unlimitedStorage
- **Purpose**: Use chrome.storage.local API to persist wallet data locally on your device
- **Stored Content**:
  - Encrypted private keys and seed phrases (using AES-GCM encryption)
  - Account list and balance cache
  - Network configuration and RPC endpoint settings
  - Connected sites list
  - Transaction history
- **Security Measures**: All sensitive data is encrypted using AES-GCM encryption algorithm, with key derivation using scrypt algorithm, ensuring that even if your device is stolen, the plaintext data cannot be read
- **Data Location**: All data is stored only on your local device and is not uploaded to any server

### tabs
- **Purpose**: Manage browser tabs for the following scenarios
- **Specific Usage**:
  - Open welcome page on first install (chrome.tabs.create)
  - Query current tabs to send messages (chrome.tabs.query)
  - Notify content scripts to disconnect (chrome.tabs.sendMessage)
- **Privacy Protection**: We do not read or record your browsing history, only communicate with specific tabs when necessary

### alarms
- **Purpose**: Implement auto-lock timer functionality
- **Specific Usage**:
  - Create timers (chrome.alarms.create)
  - Clear timers (chrome.alarms.clear)
  - Listen for timer triggers (chrome.alarms.onAlarm)
- **Feature Description**: When your set auto-lock time expires, the wallet will automatically lock to protect your assets

### <all_urls> host permission
- **Purpose**: Inject Web3 provider (window.ethereum) into websites you visit
- **Specific Usage**:
  - Content script injection: Inject Web3 provider interface when web pages load
  - RPC calls: Send transactions and query requests to blockchain nodes (e.g., Infura, Alchemy)
  - Block explorer API: Query transaction status and account information (e.g., Etherscan)
- **Accessed Hosts**:
  - All websites you actively visit (for Web3 provider injection)
  - Blockchain RPC endpoints (for sending transactions and queries)
  - Block explorer APIs (for querying on-chain data)
- **Privacy Commitment**: This is standard functionality for all Web3 wallets. We **do not collect your browsing history or website data**, only interact with websites when you actively connect your wallet

## 5. Data Security
We use local encryption and auto-lock mechanisms to protect your data. Please keep your seed phrase and password safe; lost credentials cannot be recovered.

## 6. Data Deletion
You can reset the wallet or clear extension data to remove all local data. This action is irreversible. Please back up your seed phrase in advance.

## 7. Contact Us
If you have privacy questions, please contact:  
Email: info@luckbit.link  
Team: luckbit  
Privacy Policy URL: https://victorlee2077.github.io/luckbit_docs/privacy-policy.en.html
