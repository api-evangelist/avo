# AVO

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
