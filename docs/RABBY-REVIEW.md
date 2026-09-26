# QuantumPools — targeted Rabby origin review

This is a project-prepared review packet, not an approved listing or a claim that Rabby's warning has been removed.

## Project identity

- Name: QuantumPools
- Canonical dApp origin: https://app.quantumpools.io
- Main website: https://quantumpools.io
- Official X: https://x.com/QuantumPoolsIO
- Contact: admin@quantumpools.io
- Public project information: https://github.com/Kittrian/quantumpools-public
- Structured identity: https://github.com/Kittrian/quantumpools-public/blob/main/identity.json
- Logo: https://raw.githubusercontent.com/Kittrian/quantumpools-public/main/assets/logo-400.png
- General listing packet: [WALLET-LISTING.md](WALLET-LISTING.md)

QuantumPools is a multi-chain liquidity-pool management and analytics application for concentrated-liquidity bookkeeping, fees, impermanent loss, and deposit-versus-hold performance analysis. Venue coverage includes Uniswap, PancakeSwap, Aerodrome, Raydium, Orca, and Meteora; indexing and management capabilities vary by venue and network.

## Observed warning and code trace

The reported Rabby warning reads: "The website has not been listed on any community platforms".

In Rabby's public security engine, connection rule **1004** returns `origin.communityCount` and the default warning threshold includes zero. The reviewed client sets this count to `collect_list.length` from `getOriginThirdPartyCollectList(origin)`. It also falls back to an empty list when that API request fails. Therefore the warning alone does not distinguish a genuinely empty server-side listing result from a failed lookup.

Other rules are separate:

- **1005:** site popularity.
- **1007:** the current user's personal Trusted designation.
- **1070:** Rabby verification, obtained from `isOriginVerified(origin)`.

A personal Trusted mark is not project-wide Rabby verification. Publishing this repository or adding metadata does not directly set any of Rabby's server-side values.

## Requested review

Please review `https://app.quantumpools.io` as the canonical QuantumPools origin and associate `https://quantumpools.io` with the same project identity.

1. Confirm whether the third-party listing lookup succeeds for both origins and whether the app subdomain must be mapped separately.
2. Identify the community sources that currently qualify for the returned `collect_list`, and whether an accepted source listing must include the exact app subdomain.
3. Advise the current ownership-verification and project-review requirements for Rabby's verified-origin status, where the project is eligible.
4. Retain accurate third-party DEX contract identities and all genuine transaction/security warnings. This request is for origin attribution and review, not bypassing safeguards.

No claim is made that a named directory is a Rabby data source unless Rabby confirms it. No third-party TVL, user-count, audit, or wallet-approval claim is part of this request. Production source remains private; this repository contains project information and branding only.

## Primary-source references

Reviewed September 26, 2026 (UTC). These source files may change after review.

- [Rabby security-engine connection rules](https://github.com/RabbyHub/rabby-security-engine/blob/0e1009b94f9ba724af8fe789592e916634c09498/src/rules/connect.ts)
- [Rabby client connection lookup](https://github.com/RabbyHub/Rabby/blob/e2b98a27e9ef979ab121e81e591fcf5ad79d6e19/src/ui/views/Approval/components/Connect/ConnectContent.tsx)

This packet does not report the live API values for QuantumPools; they were not successfully measured in the review session.
