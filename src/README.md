# Introduction

In order to create the first decentralized credit bureau Masa implements a set of soulbound NFT Tokens using the ERC-1155 standard. The following components are attributed to a users account during each step of the lending lifecycle. Metadata attributed to a soulbound token encrypted and can only be accessed with permission from the owner through the Masa API. 

## Identity

The Masa Identity is a soulbound NFT Identity that is generated for a user when they sign up to the Masa protocol and includes the following information:

## Credit Report

The Masa NFT Credit Report enables the bridging and aggregation of on and off-chain data in order to create a hybrid decentralized credit report. The Masa credit report can include the following information depending on which region you are located (read a a full list of supported countries here): 

- Credit Bureau Data
- Bank Transaction Data
- Mobile Money Data
- On-chain Data
- Centralized Exchange Data

## Tokenized Loan Applications

Masa tokenizes all loan applications that are attributed to a Masa Indentity and users account as a soulbound token. Once a loan application is approved a tokenized loan is created.

## Tokenized Loans

Masa tokenizes all loans that are attributed to a Masa Identity and users account. Loan applications can have the following states that get updated throughout their lifecycle: 

- pending
- approved
- disapproved
- on-time
- repaid
- late-30
- late-60
- late-90
- collections
- defaulted

# Masa API

Masa’s souldbound NFTs have their metadata stored in the Masa API which is updated in real time with verified data throughout the lifecycle of the user. The Masa API has the following endpoints available with metadata data schema’s for attribution to the souldbound NFT’s URI. 

## Identity

### Metadata URI

`https://api.masa.finance/v1.0/identity/`

### **JSON Schema**

A unique JSON schema is created for each user with the following format. 

`https://api.masa.finance/v1.0/credit-report/{id}.json`

Where `{id}` is a unique 32 character ID that is numeric characters only

Token ID’s for Identity have the `1` prefix for the TokenID and metadata `{ID}`

`10000000000000000000000000000000`

## Credit Report

### Metadata URI

`https://api.masa.finance/v1.0/credit-report/`

### **JSON Schema**

A unique JSON schema is created for each user with the following format. 

`https://api.masa.finance/v1.0/credit-report/{id}.json`

Where `{id}` is a unique 32 character ID that is numeric characters only

Token ID’s for Identity have the `2` prefix for the TokenID and metadata `{ID}`

`20000000000000000000000000000000`

## Tokenized Loan Applications

### Metadata URI

`https://api.masa.finance/v1.0/loan-applications/`

### **JSON Schema**

A unique JSON schema is created for each user with the following format. 

`https://api.masa.finance/v1.0/loan-applications/{id}.json`

Where `{id}` is a unique 32 character ID that is numeric characters only

Token ID’s for Tokenized Loan Applications have the `3` prefix for the TokenID and metadata `{ID}`

`30000000000000000000000000000000`

## Tokenized Loans

### Metadata URI

`https://api.masa.finance/v1.0/loans/`

### **JSON Schema**

A unique JSON schema is created for each user with the following format. 

`https://api.masa.finance/v1.0/loans/{id}.json`

Where `{id}` is a unique 32 character ID that is numeric characters only

Token ID’s for Tokenized Loans have the `4` prefix for the TokenID and metadata `{ID}`

`40000000000000000000000000000000`