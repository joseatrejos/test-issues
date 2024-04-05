---
name: Reporte de bug
description: Creación de un reporte de bug para mejorar nuestros software
about: Reporte de bug para Issirmax
title: "[Bug]"
labels: bug
labels: [🐛bug]
#assignees: [srinivaspendem, pushya22]
body:
- type: markdown
  attributes:
    value: |
      Thank you for taking the time to fill out this bug report.
- type: date
  attributes:
    label: Fecha de ejecución de la prueba
    description: Fecha de ejecución de la prueba
    placeholder: Fecha
- type: textarea
  attributes:
    label: Current behavior
    description: A concise description of what you're experiencing and what you expect
    placeholder: |
      When I do <X>, <Y> happens and I see the error message attached below:
      ```...```
      What I expect is <Z>
  validations:
    required: true
- type: textarea
  attributes:
    label: Steps to reproduce
    description: Add steps to reproduce this behaviour, include console or network logs and screenshots
    placeholder: |
      1. Go to '...'
      2. Click on '....'
      3. Scroll down to '....'
      4. See error
  validations:
    required: true
- type: dropdown
  id: env
  attributes:
    label: Environment
    options:
      - Production
      - Deploy preview
  validations:
    required: true
- type: dropdown
  id: browser
  attributes:
    label: Browser
    options:
      - Google Chrome
      - Mozilla Firefox
      - Safari
      - Other
- type: dropdown
  id: version
  attributes:
    label: Version
    options:
      - Cloud
      - Self-hosted
      - Local
  validations:
    required: true
