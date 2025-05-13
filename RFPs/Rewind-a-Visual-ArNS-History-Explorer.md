**Title:** Rewind - a Visual ArNS History Explorer  
**Author(s):** [JonnieSparkles](https://x.com/jonniesparkles)  
**Issue Date:** 2025-05-07  
**Submission Deadline:** 2025-06-07  
**Review and Award Period:** Two weeks  
**Expected Development Timeframe:** 2-3 Months from grant award  
**Grant Level:** Medium ($5,000 - $25,000)  
**Maximum Accepted Proposal:** 1  

## Project Overview

### Background

AR.IO is building the foundation for a decentralized, permanent cloud infrastructure that extends the Arweave protocol. A key innovation in this stack is the **Arweave Name System (ArNS)**, which acts not only as a decentralized domain system but also as a time-aware registry of domain-level metadata.

Unlike traditional naming systems that overwrite records, ArNS retains a **complete historical log** of each domain’s state. Every change to ownership, content mappings, resolvers, or metadata is immutable and auditable. This persistent log transforms the name system into a **decentralized time machine** for data and identity.

This “time machine” functionality is enabled by AO’s immutable, message-based smart contracts and Arweave’s permanent data layer - allowing anyone to independently reconstitute any past state of a name without permission or reliance on a centralized service.

As ArNS adoption grows, there is an increasing need for accessible interfaces that allow users to explore this historical data in a human-friendly and verifiable way.

### Objectives & Opportunity

The purpose of this project is to **build an open, visual explorer** for ArNS name histories that empowers users to audit, trace, and understand the evolution of any ArNS name across time.

This tool will be useful for:

- **Users** seeking transparency on ownership and updates
    
- **Developers and operators** that want to integrate deeper ArNS insights
    
- **Auditors and researchers** verifying historical records or conflicts
    

The opportunity lies in creating a public good that demonstrates the power of permanent, auditable naming and identity - made accessible and visual. This project will also serve as a reference implementation for leveraging ArNS and AO-based name history in other apps.

## Example User Story

A user discovers their favorite permaweb application, ar://totallysafe, recently introduced invasive privacy changes or, worse, became compromised by malware - echoing incidents like the January 2025 Safe multisig hack. Using the ArNS Rewind tool, the user visually navigates to an earlier, trusted version of the app, instantly restoring confidence and control over their data and the app's functionality.

## Scope of Work

### Deliverables

Proposals should aim to deliver the following:

- **Interactive History Viewer:**
    
    - A visual web-based explorer for ArNS names inspired by [https://www.ensvolution.xyz/](https://www.ensvolution.xyz/) with a scrollable or zoomable timeline, change tracking, and “click-to-inspect” functionality. Proposals that offer modular frontend components (e.g. embeddable widgets or API-driven headless interfaces) will be given special consideration.
        
- **Timeline Interface:**
    
    - Clearly displays changes to ownership, purchase type, pointers, ANT process IDs, metadata, and undernames.
        
- **Time-Based State Retrieval**
    
    - Enables users to view any ArNS name’s exact state - including metadata and mappings - at a chosen historical timestamp.
        
- **Open-source & Composable Architecture:**
    
    - All project code must be [open source](https://github.com/ar-io/ar-io-grants?tab=readme-ov-file#licensing), designed explicitly as a modular building block that can be seamlessly integrated by AR.IO gateways and other permaweb apps.
        
- **Permaweb Deployment:**
    
    - Must be a fully decentralized web app hosted on Arweave via ArNS (5+ character name lease sponsored by the Foundation) and not dependent on any single AR.IO gateway.
        
    - Use of Wayfinder protocol is encouraged.
        
- **Project Branding (Optional):**
    
    - Applicants may propose a project name or branding for their implementation. “Rewind” is used here as a working title, but creative alternatives are welcome.
        

Deliverables may also include documentation, developer APIs for integration, and optional UI enhancements (diff view, export functions, or comparison modes).

### Out of Scope

While forward-thinking development is encouraged, the following items are **not within the scope** of this initial grant and should not be prioritized:

- **Mobile app or deep mobile optimization**
    
    - Basic responsiveness is welcome, but full mobile-first UX or native mobile features are not required as this initial stage is intended for interaction on desktop via web browser.
        
- **Core protocol or registry changes**
    
    - This RFP is not for creating a new registry or modifying the underlying ArNS protocol. It is focused on creating tooling that **interfaces with** existing smart contract and AO state data.
        
- **Wallet Connectivity**
    
    - This tool is meant to be publicly accessible and permissionless. Wallet-based features like login, custom dashboards, or personalization are not required.
        

### Technical Specifications

Solutions should be compatible with the AR.IO tech stack. Proposals may leverage:

- **ArNS and ANT Process history** for time-based state evaluation
    
- **Arweave base layer** and GraphQL queries for historical contract interactions
    
- **ArNS registry and ANT process** states retrieved via AO CUs or SDKs
    
- **UI technologies** like React, Svelte, or others appropriate for data-rich, interactive timelines and web browser compatibility
    
- **Trusted published state snapshots** and/or local performance optimizations (e.g. Redis, SQLite, WASM workers) to improve resolution speed and historical lookups. IndexedDB in browser may also be utilized.
    

## Evaluation Criteria

Proposals will be evaluated based on the following:

- **Clarity & Feasibility**: How well the proposal communicates the approach, architecture, and deliverables.
    
- **Alignment with AR.IO Ethos**: Emphasis on decentralization, openness, modularity, and interoperability.
    
- **Technical Merit**: Use of AR.IO, AO, Arweave, and adherence to existing permaweb patterns.
    
- **UX & Accessibility Considerations**: Clear prioritization of user experience and accessibility.
    
- **Potential for Ecosystem Reuse**: How well the solution can serve as a building block for other projects.
    
- **Team Competency**: We welcome both solo devs and small teams with relevant experience in decentralized technologies, open-source work, or the permaweb.
    
- **Maintenance & Support Plan**: Willingness to provide documentation and continue improving the project based on feedback after initial deliverables. Preference may be given to proposals that see this as a foundation for ongoing development beyond this first phase.
    

## Resources

- 📖 [AR.IO White Paper](https://whitepaper.ar.io)
    
- 🕰️ [Building a Rewindable Internet with ArNS](https://jonniesparkles.arweave.net/articles/building-a-rewindable-internet-with-arns.html)
    
- 🏗️ [ar-io/ar-io-sdk](https://github.com/ar-io/ar-io-sdk)
    
- 💬 [AR.IO Discord](https://discord.com/invite/HGG52EtTc2) – Join the `#grants` channel
    

## How to apply?

To submit a proposal, create an issue on this repository using the "Open Proposal" issue template provided.

Proposals will be evaluated together once the general submission deadline is reached, whereby the reviewers for the RFP may provide feedback seeking clarification and amendments to your proposal before a final decision is made.

If you have questions regarding this RFP please reach out in the `#grants` channel in our Discord or [email](mailto:grants@ar.io?subject=Grants%20Inquiry) us directly.

## Terms and Conditions

- The AR.IO Foundation reserves the right to accept or reject any proposal.
    
- Multiple proposals may be selected if determined to be in the best interest of the ecosystem.
    
- The AR.IO Foundation may cancel this RFP at any time.
    
- Payment will be milestone-based. Proposed milestones and associated deliverables must be clearly outlined in the proposal.
    
- Payment will be made in ARIO tokens based on the exchange rate at time of milestone completion.
    
- All work must follow the licensing guidelines as explained in the [grants framework](https://github.com/ar-io/ar-io-grants?tab=readme-ov-file#licensing).