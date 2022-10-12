# Masa Protocol Soulbound Token Metadata

## Identity

Endpoint: `https://metadata.masa.finance/v1.0/identity/<TokenId>.json`

See [here](./identity/metadata.json) for a sample and [here](./identity/metadata_authenticated.json) for an
authenticated example

```typescript
interface IIdentity {
  name: "Masa Soulbound Identity v1.0.0";
  description: "A self-sovereign identity for accessing DeFi";
  image: "https://metadata.masa.finance/v1.0/identity/masa-identity.png";
  properties: {
    tokenId: string;
    account?: string;
    soulName?: string;
  };
}
```

## Soul Name

The metadata for the Soul Name contract can be
found [here](https://github.com/masa-finance/masa-contracts-identity/blob/main/metadata/SoulName.json)

Endpoint: `ar://<arweave id>`

See [here](./soul-name/metadata.json) for a sample

```typescript
// tbd
```

## Credit Report

Endpoint: `https://metadata.masa.finance/v1.0/credit-report/<TokenId>.json`

See [here](./credit-report/metadata.json) for a sample and [here](./credit-report/metadata_authenticated.json) for an
authenticated example

```typescript
interface ICreditReport {
  name: "Masa Soulbound Credit Report v1.0.0";
  description: "A decentralized credit report";
  image: "https://metadata.masa.finance/v1.0/identity/credit-report.png";
  properties: {
    tokenId: string;
    account?: string;
    lastUpdated?: string;
    model_version?: string;
    value?: number;
    decile?: string;
    value_rating?: string;
  };
}
```
