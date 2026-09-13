# AgileSoDA

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

AgileSoDA (애자일소다) is a Seoul-based enterprise AI software company founded in April 2015, whose name
combines "Agility" with "Software Defined AI". It builds agentic AI systems that automate and optimize
complex business decisions for Korean enterprises across insurance, banking, manufacturing and the
public sector, and was named a Gartner Cool Vendor in 2024.

Its current line is organized around the **JT (Just Type)** platform — JT Foundry for deploying and
operating agents, JT Solution, Agentic OCR (ETL with VLM), Agentic RAG, Agentic Ops, the insurance
document extractor InsuDoc, Ground Forge for automated data annotation, and a vibe-coding UI Package.
Earlier products still carried on the documentation portal are SparklingSoDA, BakingSoDA
(reinforcement-learning decision agents), TwinDoc, TwinReader (OCR) and ModelServant.

## API surface

**No public API contract was found.** AgileSoDA sells licensed enterprise software installed in the
customer's own environment, so there is no hosted base URL, no self-service signup, no API key issuance
and no published pricing — every commercial path on the site is a contact form.

The company *does* publish a product documentation portal at
[docs.agilesoda.ai](http://docs.agilesoda.ai/agiledocs_ko). Its index is public and lists an
Installation Guide, Admin Guide, Getting Started, Developer's Guide and Use Cases Book for each product,
plus a **ModelServant API Guide** and a Server Spec Guide. Every one of those linked guides returns the
portal's username/password sign-on form instead of content, which is why this profile is recorded as
`gated / customer-only-docs`: the contract exists, but only customers can read it.

Contract discovery run 2026-09-12 against `agilesoda.ai`, `www.agilesoda.ai` and `docs.agilesoda.ai`:

| Probe | Result |
|---|---|
| `/openapi.json`, `/openapi.yaml`, `/swagger.json`, `/v1/openapi.json`, `/api-docs`, `/v2/api-docs`, `/docs`, `/redoc`, `/rapidoc`, `/swagger-ui.html`, `/api/openapi.json` | 404 on every host |
| `/graphql` introspection | 404 |
| `/mcp`, `/.well-known/mcp.json` | 404 |
| `/.well-known/agent-card.json`, `/.well-known/agent.json` | 404 — no agent card, so none is authored |
| Named `/.well-known/` + `/apis.json` path list | 404 on every path, every host (see `well-known/`) |
| npm / PyPI / crates.io / GitHub org | no first-party SDK published |
| Pricing page | `https://agilesoda.ai/pricing` → 404 |

One security note worth passing on: `docs.agilesoda.ai` has port 443 closed and serves the portal —
including its credential login form — only over plaintext HTTP. Recorded in
`security/agilesoda-domain-security.yml`.

## Links

- Website — https://agilesoda.ai/
- Documentation portal — http://docs.agilesoda.ai/agiledocs_ko
- GitHub organization — https://github.com/AgileSoda
- Contact / demo request — https://agilesoda.ai/contact
- Investor relations — https://agilesoda.ai/ir
- LinkedIn — https://www.linkedin.com/company/agilesoda
