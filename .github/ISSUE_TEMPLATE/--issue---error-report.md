name: Error report
description: Report a bug. For security vulnerabilities see Report a security vulnerability in the templates.
title: "Error: "
labels: [Error]

body:
- type: markdown
  attributes:
    value: >
      ####Thank you for taking the time to file a error report. Before creating a new issue, please make sure to take a few minutes to check the issue tracker for [existing and past issues](https://github.com/BGIResearch/SAW/issues)
      for existing issues about the bug.
    
- type: textarea
  attributes: 
    label: "Describe the issue:"
  validations:
    required: true

- type: textarea
  attributes:
    label: "Reproduce the code example:"
    description: >
      A short code example that reproduces the problem/missing feature. It
      should be self-contained, i.e., can be copy-pasted into the Python
      interpreter or run as-is via `python myproblem.py`.
    placeholder: |
      import numpy as np
      << your code here >>
    render: python
  validations:
    required: true
  
- type: textarea
  attributes:
    label: "Error message:"
    description: >
      Please include full error message, if any.
      If you are reporting a segfault please include a GDB traceback,
      which you can generate by following
      [these instructions](https://github.com/numpy/numpy/blob/main/doc/source/dev/development_environment.rst#debugging).
    placeholder: |
      << Full traceback starting from `Traceback: ...` >>
    render: shell

- type: textarea
  attributes:
    label: "NumPy/Python version information:"
    description: Output from `import sys, numpy; print(numpy.__version__, sys.version)`.
  validations:
    required: true

- type: textarea
  attributes:
    label: "Context for the issue:"
    description: |
      Please explain how this issue affects your work or why it should be prioritized.
    placeholder: |
      << your explanation here >>
  validations:
    required: false