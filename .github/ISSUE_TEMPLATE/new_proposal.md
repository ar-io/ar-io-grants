---
name: Open Proposal Template
description: Submit a new Open Proposal to to AR.IO Foundation
title: "[Open Proposal]: "
labels: ["Open Proposal"]
assignees:

body:
  - type: markdown
    attributes:
      value: |
        # Grant Application Form
        Thank you for your interest in the AR.IO Foundation Grant Program! Please fill out this form with all the required information.

  - type: markdown
    attributes:
      value: |
        ## Project Details

  - type: input
    id: project_name
    attributes:
      label: Project Name
      description: Name of your project
      placeholder: e.g. Fun Wallet
    validations:
      required: true

  - type: input
    id: team_name
    attributes:
      label: Team Name
      description: Legal name of your team
      placeholder: e.g. Fun Wallet Inc.
    validations:
      required: true

  - type: input
    id: payment_address
    attributes:
      label: ARIO Payment Address
      description: Address to receive grant funds
    validations:
      required: true

  - type: dropdown
    id: level
    attributes:
      label: Level
      description: Grant level requested
      options:
        - Level 1
        - Level 2
        - Level 3
    validations:
      required: true

  - type: input
    id: previous_grants
    attributes:
      label: Links to previous ARIO grants
      description: If applicable, include links to previous grants
      placeholder: https://github.com/organization/repo/issues/123

  - type: dropdown
    id: open_source
    attributes:
      label: Project is open-source
      options:
        - "Yes"
        - "No"
    validations:
      required: true

  - type: input
    id: project_repo
    attributes:
      label: Project Repository
      description: Link to the project repository
      placeholder: https://github.com/your-org/your-repo

  - type: markdown
    attributes:
      value: |
        ## Contact Details

  - type: input
    id: contact_name
    attributes:
      label: Contact Name
      description: Full name of the primary contact for your team
    validations:
      required: true

  - type: input
    id: contact_email
    attributes:
      label: Contact Email
      description: Email address for primary contact
      placeholder: example@email.com
    validations:
      required: true

  - type: input
    id: website
    attributes:
      label: Website
      description: Your project or organization website
      placeholder: https://yourproject.com

  - type: markdown
    attributes:
      value: |
        ## Project Overview

  - type: textarea
    id: brief_description
    attributes:
      label: Brief Description
      description: A brief description of your project
      placeholder: Describe your project in a few sentences...
    validations:
      required: true

  - type: textarea
    id: relationship_to_ario
    attributes:
      label: Relationship to AR.IO Network
      description: How does this project relate to the AR.IO Network?
      placeholder: Explain how your project connects to the AR.IO ecosystem...
    validations:
      required: true

  - type: textarea
    id: reasons_for_project
    attributes:
      label: Reasons for Project
      description: Why is your team interested in creating this project?
      placeholder: Share your motivation and goals...
    validations:
      required: true

  - type: markdown
    attributes:
      value: |
        ## Details
        Please provide a detailed overview of the project you're proposing.

  - type: textarea
    id: project_details
    attributes:
      label: Project Details
      description: Include mockups, data models, API specifications, tech stack, etc.
      placeholder: |
        Please include information such as:
        - Mock-ups/designs of any UI components
        - Data models of the core functionality
        - API specifications of the core functionality
        - An overview of the technology stack to be used
        - Documentation of core components, protocols, architecture, etc.
        - PoC/MVP or other relevant prior work or research
        - What your project is *not* or will *not* provide or implement
    validations:
      required: true

  - type: textarea
    id: ecosystem_fit
    attributes:
      label: Ecosystem Fit
      description: How does your project fit into the AR.IO ecosystem?
      placeholder: |
        Please address:
        - Where and how does your project fit into the ecosystem?
        - Who is your target audience?
        - What need(s) does your project meet?
        - Are there similar projects in the AR.IO Network / Arweave / AO ecosystem?
          - If so, how is your project different?
          - If not, are there similar projects in related ecosystems?
    validations:
      required: true

  - type: markdown
    attributes:
      value: |
        ## Team

  - type: input
    id: team_leader
    attributes:
      label: Team Leader
      description: Name of team leader
    validations:
      required: true

  - type: textarea
    id: team_members
    attributes:
      label: Team Members
      description: Names of all team members
      placeholder: |
        - Name of team member 1
        - Name of team member 2
        - Name of team member 3
    validations:
      required: true

  - type: input
    id: legal_entity
    attributes:
      label: Registered Legal Entity
      description: Name of your registered legal entity
      placeholder: e.g. Greymass, Inc.
    validations:
      required: true

  - type: input
    id: registered_address
    attributes:
      label: Registered Address
      description: Address of your registered legal entity (single line)
      placeholder: 123 Main Street, London LK1 234, UK
    validations:
      required: true

  - type: textarea
    id: team_experience
    attributes:
      label: Team Experience
      description: Describe the team's relevant experience, particularly for development work
      placeholder: |
        Please describe relevant experience and past projects.
        If anyone has applied for a grant at the ARIO Foundation previously, please list the project and legal entity.
    validations:
      required: true

  - type: textarea
    id: team_repos
    attributes:
      label: Team Organization Repositories
      description: GitHub repositories for your team/organization
      placeholder: |
        - https://github.com/<your_organization>
        - https://github.com/<your_organization>/<project_1>
        - https://github.com/<your_organization>/<project_2>
    validations:
      required: true

  - type: textarea
    id: member_repos
    attributes:
      label: Team Member Repositories
      description: GitHub accounts of all team members
      placeholder: |
        - https://github.com/<team_member_1>
        - https://github.com/<team_member_2>
    validations:
      required: true

  - type: textarea
    id: social_profiles
    attributes:
      label: Team Social Profiles
      description: Social media profiles of team members
      placeholder: |
        Person 1:
        - X: @handle
        - LinkedIn: https://linkedin.com/in/...

        Person 2:
        - X: @handle
        - LinkedIn: https://linkedin.com/in/...

  - type: markdown
    attributes:
      value: |
        ## Development Status

  - type: textarea
    id: development_status
    attributes:
      label: Development Status
      description: Current status of your project and relevant research
      placeholder: |
        Please provide:
        - Links to code repositories if you've already started implementation
        - Documentation on research and other work conducted
        - Links to improvement proposals or RFPs
        - Academic publications relevant to the problem
        - Links to research diary, blog posts, articles, forum discussions, or open GitHub issues
        - References to conversations with the ARIO Foundation
        - Previous interface iterations, such as mock-ups and wireframes
    validations:
      required: true

  - type: markdown
    attributes:
      value: |
        ## Development Roadmap
        Break down your development roadmap into milestones and deliverables.

  - type: input
    id: total_duration
    attributes:
      label: Total Estimated Duration
      description: Duration of the whole project (e.g. 2 months)
      placeholder: e.g. 2 months
    validations:
      required: true

  - type: input
    id: total_fte
    attributes:
      label: Full-Time Equivalent (FTE)
      description: Average number of full-time employees working on the project
      placeholder: e.g. 2 FTE
    validations:
      required: true

  - type: input
    id: total_costs
    attributes:
      label: Total Costs
      description: Requested amount in USD for the whole project
      placeholder: e.g. 12,000 USD
    validations:
      required: true

  - type: textarea
    id: milestone_1
    attributes:
      label: Milestone 1
      description: Details for the first milestone
      placeholder: |
        ### Milestone 1 Description
        - **Estimated duration:** 1 month
        - **FTE:** 2
        - **Costs:** 8,000 USD

        | ID | Deliverable | Specification |
        | --- | --- | --- |
        | 0a. | License | MIT / Apache 2.0 / GPLv3 / Unlicense |
        | 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial |
        | 0c. | Testing Guide | Core functions will be fully covered by unit tests with instructions |
        | 0d. | Docker | We will provide Dockerfile(s) for testing |
        | 0e. | Article | We will publish an article explaining what was achieved |
        | 1. | [Feature 1] | [Description of implementation] |
        | 2. | [Feature 2] | [Description of implementation] |
        | 3. | [Feature 3] | [Description of implementation] |
    validations:
      required: true

  - type: textarea
    id: milestone_2
    attributes:
      label: Milestone 2
      description: Details for the second milestone (if applicable)
      placeholder: |
        ### Milestone 2 Description
        - **Estimated duration:** 1 month
        - **FTE:** 2
        - **Costs:** 4,000 USD

        | ID | Deliverable | Specification |
        | --- | --- | --- |
        | 0a. | License | MIT / Apache 2.0 / GPLv3 / Unlicense |
        | 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial |
        | 0c. | Testing Guide | Core functions will be fully covered by unit tests with instructions |
        | 0d. | Docker | We will provide Dockerfile(s) for testing |
        | 0e. | Article | We will publish an article explaining what was achieved |
        | 1. | [Feature 1] | [Description of implementation] |
        | 2. | [Feature 2] | [Description of implementation] |
        | 3. | [Feature 3] | [Description of implementation] |

  - type: textarea
    id: milestone_3
    attributes:
      label: Milestone 3
      description: Details for additional milestones (if applicable)
      placeholder: "Add additional milestones as needed..."

  - type: textarea
    id: future_plans
    attributes:
      label: Future Plans
      description: Short-term and long-term plans for your project
      placeholder: |
        Please include:
        - How you intend to use, enhance, promote and support your project in the short term
        - The team's long-term plans and intentions in relation to it
    validations:
      required: true

  - type: textarea
    id: additional_info
    attributes:
      label: Additional Information
      description: Any other relevant information
      placeholder: |
        - How did you hear about the Grants Program?
        - Work you have already done
        - If there are any other teams who have already contributed (financially) to the project
        - Previous grants you may have applied for
    validations:
      required: true

  - type: checkboxes
    id: terms
    attributes:
      label: Terms and Conditions
      description: By submitting this application, you agree to the grant program terms
      options:
        - label: I understand that this application will be evaluated based on the criteria outlined in the grant framework
          required: true
        - label: I confirm that all the information provided in this application is accurate and complete
          required: true
        - label: I understand that if my grant is approved, I will be required to provide regular updates on milestone progress
          required: true
