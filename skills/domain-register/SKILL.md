---
name: domain-register
description: Register a domain autonomously on Headless Domains using Machine Payments Protocol (MPP) with pathUSD or Gems.
---

# Domain Register

This skill allows an AI agent to autonomously register a domain using Machine Payments Protocol (MPP).

## Usage

Endpoint: `POST https://headlessdomains.com/api/v1/domains/register`

### Request

- Method: `POST`
- URL: `https://headlessdomains.com/api/v1/domains/register`
- Headers:
  - `Content-Type: application/json`
- Body:
  - `domain` (string, required): The domain to register.
  - `namespace` (string, required): The namespace.
  - `years` (integer, required): Registration duration in years.
  - `agreed_to_terms` (boolean, required): Must be true.
  - `payment_method` (string, required): `mpp` or `gems`.
  - `receipt` (string, optional): MPP payment authorization receipt (if challenged).

### Payment Flow (MPP)

1. Send the initial POST request without a `receipt`.
2. Receive a `402 Payment Required` challenge.
3. Fulfill the payment and obtain a receipt.
4. Re-submit the POST request including the `receipt`.

### Example Request

```bash
curl -X POST https://headlessdomains.com/api/v1/domains/register \
  -H "Content-Type: application/json" \
  -d '{"domain": "myagent", "namespace": "agent", "years": 1, "agreed_to_terms": true, "payment_method": "mpp"}'
```
