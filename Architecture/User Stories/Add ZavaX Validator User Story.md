## **User Story: Adding a ZavaX Validator**

### **As** a ZAX Owner,

**I want to** initiate the process of becoming a ZavaX subnet validator through the Avalanche command line interface,

**So that** I can be a part of the ZavaX validator network, in order to later become a ZavaX bridge warden, contributing to the security and operation of the ZavaX bridge.

---

### **Flow**:

1. **Initialization**:
    - **Given** I am a ZAX Owner,
    - **When** I initiate the validation process through the Avalanche-cli,
    - **Then** the Avalanche-cli requests a transaction signature from my Ledger device.

2. **Ledger Interaction**:
    - **Given** a signature request is sent to the Ledger,
    - **When** my Ledger prompts me for approval,
    - **And** I approve the transaction,
    - **Then** my Ledger signs the transaction.

3. **Completion of Validation Request**:
    - **Given** the Ledger has signed the transaction,
    - **When** the signed transaction is returned to the Avalanche-cli,
    - **And** the Avalanche-cli submits the validation request to the Avalanche P-Chain,
    - **Then** I receive a response indicating the status of my validation request.

