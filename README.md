# Headless Domains Agent Skills

[![Agent Skills](https://skills.sh/b/headlessdomains/skills)](https://skills.sh/headlessdomains/skills)

Welcome to the **Headless Domains** Agent Skills repository. These skills provide "Agentic SEO" and machine-discoverability for the Headless Domains platform, allowing autonomous AI agents to seamlessly interact with our API.

## About

Headless Domains is an Agentic Domain Registrar. We expose core API capabilities as discrete "skills" so that agents can search, look up, register, and sync bios for decentralized domains.

- **Author/Owner:** headlessdomains
- **Project URL:** [https://headlessdomains.com](https://headlessdomains.com)
- **OpenAPI Spec:** [https://headlessdomains.com/openapi.json](https://headlessdomains.com/openapi.json)

## Available Skills

1. **`domain-search`**: Check if a domain name is available for registration across all supported namespaces.
2. **`domain-lookup`**: Retrieve public profile information, active capabilities, and agentic commerce storefront details for a given domain.
3. **`domain-register`**: Register a domain autonomously using Machine Payments Protocol (MPP) with pathUSD or Gems.
4. **`bio-sync`**: Synchronize or update the decentralized bio/profile for a specific domain.

## Installation

These skills conform to the `skills.sh` standard. To install them for your autonomous agent, simply run:

```bash
npx skills add headlessdomains/skills
```

You can also specify a single skill to install:

```bash
npx skills add headlessdomains/skills --skill domain-search
```

## Contributing

For details on the API contracts and further integration possibilities, please refer to our [OpenAPI Spec](https://headlessdomains.com/openapi.json).
