# Documentation project instructions

## About this project

- Documentation site for the Biznet GIO Infrastructure-as-Code providers, built on [Mintlify](https://mintlify.com)
- Deployed at https://biznetgio.creations.ren
- Pages are MDX files with YAML frontmatter; configuration lives in `docs.json`
- Preview locally with `mint dev` (run at the repo root, view at http://localhost:3000)

## Covered products

- Terraform provider: https://github.com/shirasakaren/terraform-provider-biznetgio
- Pulumi provider: https://github.com/shirasakaren/pulumi-biznetgio
- Upstream API reference: https://api.portal.biznetgio.com/v1/docs

## Terminology

- "NEO Lite" and "NEO Lite Pro" (capitalized, space-separated) — the VPS products; code-level identifiers are `neolite` / `neolite_pro`
- "NEO Metal" — bare-metal; "NEO GPU" — GPU instances; "NEO Object Storage" — S3-compatible storage; "NES" — NEO Elastic Storage
- API token, not API key, in prose (config attribute is `api_key` / `apiToken`)
- Attribute names in code formatting (`disk_size`), Terraform snake_case vs Pulumi camelCase (`diskSize`) as appropriate

## Style preferences

- Active voice, second person ("you")
- Sentence case headings; one idea per sentence
- Reference pages use tables for schemas — tables carry the detail, prose stays short
- Frontmatter `title` + `description` on every page; descriptions are one sentence
- Real links only — no placeholders anywhere

## Content boundaries

- Document only the five API groups the providers cover: neolites, neolite-pros, baremetals (+additional-ips, +elastic-storages), neo-gpus, object-storages
- Do not document portal UI-only features or products without a public API
