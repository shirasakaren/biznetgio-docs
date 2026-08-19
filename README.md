# BiznetGIO Providers Docs

Documentation for the [Biznet GIO](https://biznetgio.com) cloud providers — Terraform and Pulumi — built with [Mintlify](https://mintlify.com).

- Deployed at: https://biznetgio.creations.ren
- Terraform provider: https://github.com/shirasakaren/terraform-provider-biznetgio
- Pulumi provider: https://github.com/shirasakaren/pulumi-biznetgio

## Structure

- `docs.json` — site configuration (navigation, branding, links)
- `index.mdx`, `quickstart.mdx`, `pulumi-quickstart.mdx`, `authentication.mdx` — getting started
- `terraform/` — Terraform provider reference (installation, resources per service, importing)
- `pulumi/` — Pulumi provider reference (installation, resources per service, importing)
- `guides/` — billing, triggers, development, FAQ
- `logo/` + `favicon.svg` — brand assets

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint):

```bash
npm i -g mint
```

Preview locally (at the repo root, where `docs.json` lives):

```bash
mint dev
```

View the preview at http://localhost:3000. Run `mint update` if the dev environment is outdated.

## Publishing

Changes pushed to the default branch deploy automatically via the Mintlify GitHub app.

## License

Apache-2.0 — see [LICENSE](LICENSE).
