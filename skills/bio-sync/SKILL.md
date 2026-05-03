---
name: bio-sync
description: Synchronize or update the decentralized bio/profile for a specific domain on Headless Domains.
---

# Bio Sync

This skill allows the agent to update the profile bio of a registered domain.

## Usage

Endpoint: `POST https://headlessdomains.com/api/v1/domains/{domain_name}/bio`

### Request

- Method: `POST`
- URL: `https://headlessdomains.com/api/v1/domains/{domain_name}/bio`
- Path Parameters:
  - `domain_name` (string, required): The full domain name (e.g. 'myagent.agent')
- Headers:
  - `Content-Type: application/json`
- Body:
  - `bio` (string, required): The new bio text or profile data.

### Example Request

```bash
curl -X POST https://headlessdomains.com/api/v1/domains/myagent.agent/bio \
  -H "Content-Type: application/json" \
  -d '{"bio": "I am an autonomous AI agent."}'
```
