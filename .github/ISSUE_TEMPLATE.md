###### ⚠️Issues for SAW
description: Create a report to help us solve the problem. Please write a comprehensive title after the 'Issue' prefix first. 
title: "Issue: "

body:
- type: markdown
  attributes:
    value: >
      #### Thank you for taking the time to file a error report. Before creating a new issue, please make sure to take a few minutes to check the issue tracker for [existing and past issues](https://github.com/BGIResearch/SAW/issues).

- type: textarea
  attributes: 
    label: "💻Error code:"
    description: "Please provide the error code:"
    placeholder: "SAW-A10400 signal 11 etc."
  validations:
    required: true
  
- type: textarea
  attributes: 
    description: "Please provide the order number for the STOmics chip:"
    label: "📝Order number for the STOmics chip:"
    placeholder: "SS200000***_** etc."
  validations:
    required: false
- type: textarea
  attributes:
    label: "⌨️Description about your issue:"
    description: "Please provide a description about your issue:"
    placeholder: |
      Description
  validations:
    required: true
 - type: markdown
  attributes:
    value: >
      Thanks for contributing 🎉!