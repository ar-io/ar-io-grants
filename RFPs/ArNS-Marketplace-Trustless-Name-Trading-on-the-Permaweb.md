**Title:** ArNS Marketplace - Trustless Name Trading on the Permaweb  
**Author(s):** [Vilenarios](https://x.com/vilenarios), [JonnieSparkles](https://x.com/jonniesparkles), 
**Issue Date:** 2025-05-08
**Submission Deadline:** 2025-06-08
**Review and Award Period:** Two weeks
**Expected Timeframe:** 8-12 weeks  
**Grant Level:** Large ($25,000 - $50,000)  
**Maximum Accepted Proposal:** 1

### Project Overview

**Background**

The Arweave Name System (ArNS) enables users to register friendly, permanent domain names for permaweb content, identities, sites, and applications. These names are represented by Arweave Name Tokens (ANTs), which are smart contracts powered by the AO Computer. ANTs are unique, transferrable, and tradable; however, there is currently no decentralized secondhand marketplace where users can trustlessly buy, sell, or auction registered names.

**Objectives & Opportunity**

This project seeks to deliver a trustless, decentralized ArNS marketplace that allows:

- Name owners to list their ArNS names for sale via buy-it-now, Dutch auction, or English auction
- Buyers to purchase names directly or bid in auctions
- Safe, on-chain ANT ownership transfer via AO processes and escrow

This RFP does not prescribe a specific architecture or auction protocol. Applicants are encouraged to propose and justify innovative technical approaches that meet the trustlessness and decentralization goals.

The marketplace will make the ArNS namespace more accessible, valuable, and usable across the ecosystem.
### Scope of Work

**Deliverables**

- Fully functional marketplace web application deployed via Arweave and accessible at an `ar://` ArNS name
- ArNS Marketplace smart contract(s)/AO process(es) to manage listings, escrow, and settlements
- Seller UI to list ArNS names, define price/auction parameters, and cancel active listings
- Buyer UI to browse listings, bid/purchase, and view past auctions
- Wallet support: login with Arweave wallet (Wander) and Ethereum wallet (MetaMask)
- Name ownership verification system via AO to ensure only rightful ANT owners can list
- Escrow logic to transfer ARIO tokens to sellers upon sale completion
- ANT transfer mechanism via reassignment or pre-signed mutation
- Indexing and search mechanism for marketplace listings
- Documentation and deployment guide

### Technical Specifications

- Must be hosted entirely on the Permaweb (Arweave)
- Must use ArNS for its primary domain (e.g. `market.ar.io`). Note that a 5+ character name lease may be sponsored by the Foundation.
- Must support ANT ownership via the ArNS and AO smart contract standards
- Must use AO for escrow logic (can build new or reuse protocols like FusionFi)
- Must use ARIO token for all payments in v1
- Must follow AR.IO SDK and ArNS registry protocols for name interactions
- Must ensure no admin keys or centralized control of user funds or names

### Evaluation Criteria

Proposals will be evaluated based on:

- Technical quality and architecture
- Demonstrated understanding of ArNS and AO
- UX design and ease of use
- Trustlessness and decentralization
- Feasibility of timeline and deliverables
- Team experience and past work
- Long-term maintainability and extensibility

The author(s) of this RFP will participate in reviewing proposals.

## Resources

- 📖 [AR.IO White Paper](https://whitepaper.ar.io)
- 🏗️ [ar-io/ar-io-sdk](https://github.com/ar-io/ar-io-sdk)
- 🧪 [Early POC via Bazar](https://docs.ar.io/guides/ants-on-bazar)
- 💬 [AR.IO Discord](https://discord.com/invite/HGG52EtTc2) – Join the #grants channel

## How to apply?
  
To submit a proposal, create an issue on this repository using the "Open Proposal" issue template provided.
  
Proposals will be evaluated together once the general submission deadline is reached, whereby the reviewers for the RFP may provide feedback seeking clarification and amendments to your proposal before a final decision is made.

If you have questions regarding this RFP please reach out in the grants channel in our Discord or [email](mailto:grants@ar.io?subject=Grants%20Inquiry) us directly.

## Terms and Conditions

- The AR.IO Foundation reserves the right to accept or reject any proposal.
- Multiple proposals may be selected if determined to be in the best interest of the ecosystem.
- The AR.IO Foundation may cancel this RFP at any time.
- Payment will be milestone-based. Proposed milestones and associated deliverables must be clearly outlined in the proposal.
- Payment will be made in ARIO tokens based on the exchange rate at time of milestone completion.
- All work must follow the licensing guidelines as explained in the [grants framework](https://github.com/ar-io/ar-io-grants?tab=readme-ov-file#licensing).