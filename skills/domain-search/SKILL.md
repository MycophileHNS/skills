---
name: domain-search
description: Check if a domain name is available for registration on Headless Domains.
---

# Domain Search

This skill allows the agent to search for available domains on the Headless Domains platform.

## Usage

Endpoint: `GET https://headlessdomains.com/api/v1/domains/search?q={query}`

### Request

- Method: `GET`
- URL: `https://headlessdomains.com/api/v1/domains/search`
- Query Parameters:
  - `q` (string, required): The domain name to search (e.g. 'myagent' or 'myagent.agent')

### Example Request

```bash
curl -s "https://headlessdomains.com/api/v1/domains/search?q=myagent"
```
