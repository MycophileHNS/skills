---
name: domain-lookup
description: Retrieve public profile information, active capabilities, and agentic commerce storefront details for a given domain on Headless Domains.
---

# Domain Lookup

This skill allows the agent to look up a domain profile on the Headless Domains platform.

## Usage

Endpoint: `GET https://headlessdomains.com/api/v1/lookup/{domain_name}`

### Request

- Method: `GET`
- URL: `https://headlessdomains.com/api/v1/lookup/{domain_name}`
- Path Parameters:
  - `domain_name` (string, required): The full domain name to look up (e.g. 'myagent.chatbot')

### Example Request

```bash
curl -s "https://headlessdomains.com/api/v1/lookup/myagent.chatbot"
```
