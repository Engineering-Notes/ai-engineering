# Engineering Notes: AI Engineering

[![CI](https://github.com/Engineering-Notes/ai-engineering/actions/workflows/ci.yml/badge.svg)](https://github.com/Engineering-Notes/ai-engineering/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Node.js 22](https://img.shields.io/badge/node-22-339933.svg)](.nvmrc)

Evaluations, retrieval, agents and the economics of models in production, measured.

Tested code behind the **AI Engineering** series of [Engineering Notes](https://github.com/Engineering-Notes), published on [codemwangi.substack.com](https://codemwangi.substack.com). The series starts on February 2027. Every number quoted in an article will come from the code in its folder, and CI runs all of it on every change.

## Articles

The article list will be published here before the series starts. Topic proposals are welcome in [Discussions](https://github.com/orgs/Engineering-Notes/discussions).

## Running an article

Each article lives in its own folder, `NN-name`, with its own `package.json`, lockfile and tests.

```bash
git clone https://github.com/Engineering-Notes/ai-engineering.git
cd ai-engineering
docker compose up -d        # PostgreSQL 16, for the articles that need it
cd 01-<name>
npm ci
npm test
```

`npm test` exits with an error if the approach an article recommends ever produces a wrong result.

## Related

- [Payment Systems](https://github.com/Engineering-Notes/payment-systems), the first series.
- [Contributing](https://github.com/Engineering-Notes/.github/blob/main/CONTRIBUTING.md), [code of conduct](https://github.com/Engineering-Notes/.github/blob/main/CODE_OF_CONDUCT.md) and [security policy](https://github.com/Engineering-Notes/.github/blob/main/SECURITY.md) apply to this repository.

## Licence

[MIT](LICENSE)
