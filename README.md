# AVO

Avo (avonow.com) was a New York City-based "building commerce" and workplace-amenity platform, founded 2017-2018 out of Y Combinator (S18) and backed by Insight Partners and Kleiner Perkins with roughly $84M raised. It offered white-labeled same-day delivery of groceries, household goods, alcohol and personal-care items into residential and office buildings with no order minimums or delivery fees, plus on-site and virtual event programming and corporate gifting and recognition services, serving apartment communities, corporations, hospitals and universities across New York, New Jersey, Chicago and Houston.

Backed by: insight-partners — https://www.avonow.com/

## API surface

None. AVO published no API, SDK, CLI, developer portal or public developer documentation.

As of a 2026-07-20 enrichment probe:

- `www.avonow.com` returns an identical 114-byte GoDaddy parking redirect for **every** path, including a control path that does not exist — a soft-404, so no `/.well-known/` document is actually published.
- No operational subdomains resolve (`oms`, `app`, `shop`, `admin`, `backend`, `static`).
- Y Combinator lists the company as inactive.

The domain still carries valid TLS (TLSv1.3), SPF and a DMARC `quarantine` policy, but no HSTS, DNSSEC or CAA.

## Artifacts

| Artifact | File | Method |
|---|---|---|
| Domain security | `security/avo-domain-security.yml` | probed |
| Well-known probe (negative result) | `well-known/avo-well-known.yml` | probed |
| llms.txt | `llms/avo-llms.txt` | generated |
