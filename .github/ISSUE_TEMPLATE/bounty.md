---
name: Bounty Submission
description: Submit a new bounty or apply for an existing one
title: "[BOUNTY]: "
labels: ["bounty", "Accepting Applications"]
assignees:
  - octocat
body:
  - type: markdown
    attributes:
      value: |
        # Bounty Submission Form
        Thank you for your interest in our bounty program! Please fill out the information below.
  
  - type: dropdown
    id: status
    attributes:
      label: Status
      description: Current status of this bounty
      options:
        - Accepting Applications
        - Bounty Assigned
        - Bounty Completed
    validations:
      required: true
  
  - type: input
    id: deciders
    attributes:
      label: Deciders
      description: Grant Committee Members who will review applications
      placeholder: "@username1, @username2"
    validations:
      required: true
  
  - type: input
    id: date
    attributes:
      label: Date
      description: Date of bounty creation
      placeholder: YYYY-MM-DD
    validations:
      required: true
  
  - type: input
    id: authors
    attributes:
      label: Authors
      description: Who authored this bounty
      placeholder: "@username"
    validations:
      required: true
  
  - type: textarea
    id: summary
    attributes:
      label: General Summary
      description: Provide a brief summary of the bounty being offered
      placeholder: Describe the bounty in a few sentences...
    validations:
      required: true
  
  - type: textarea
    id: reward
    attributes:
      label: Reward
      description: Please detail the reward that is being offered for this bounty.
      placeholder: E.g., $X,XXX USD paid in ARIO Tokens
    validations:
      required: true
  
  - type: textarea
    id: requirements
    attributes:
      label: Requirements
      description: Please detail the requirements for a successful completion of this bounty
      placeholder: List all requirements and acceptance criteria...
    validations:
      required: true
      
  - type: textarea
    id: timeline
    attributes:
      label: Timeline
      description: Expected timeline for completion
      placeholder: E.g., 2 weeks from assignment
    validations:
      required: true
      
  - type: dropdown
    id: size
    attributes:
      label: Bounty Size
      description: Size/complexity of this bounty
      options:
        - Small
        - Medium
        - Large
    validations:
      required: true