# Simple Tool Rental API – Automated Tests

![API Tests](https://github.com/matibarluenga/tool-rental-api-tests/actions/workflows/api-tests.yml/badge.svg)

Automated API tests for the [Simple Tool Rental API](https://simple-tool-rental-api.click) built with **Postman** and run with **Newman** in **GitHub Actions** on every push and pull request.

## What's covered

- **Tools**
  - `GET /tools`: status code, response time, and required fields on every item

## Tech stack

- Postman (collection + environment)
- Newman + newman-reporter-htmlextra
- GitHub Actions

## Run locally

```bash
npm ci
npm test
```

The HTML report is generated at `reports/report.html`.

## CI

Each run uploads the HTML report as the `newman-report` artifact (available in the Actions tab).

## Notes

Tests run against a public third-party API, so occasional failures may be caused by the service being unavailable.
