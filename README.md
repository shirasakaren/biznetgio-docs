<p align="center">
  <img src="./logo/light.svg" width="220" alt="BiznetGIO Providers docs" />
</p>

<h1 align="center">BiznetGIO Providers Docs</h1>

<p align="center">
  Documentation for the Biznet GIO Terraform and Pulumi providers, built with <a href="https://mintlify.com">Mintlify</a>.
</p>

<p align="center">
  <a href="https://github.com/shirasakaren/biznetgio-docs/deployments"><img src="https://img.shields.io/github/deployments/shirasakaren/biznetgio-docs/production?label=deploy" alt="Deployment"></a>
  <a href="./LICENSE"><img src="https://img.shields.io/github/license/shirasakaren/biznetgio-docs" alt="License"></a>
  <a href="https://github.com/shirasakaren/biznetgio-docs"><img src="https://img.shields.io/github/stars/shirasakaren/biznetgio-docs?style=social" alt="GitHub stars"></a>
</p>

<p align="center">
  <a href="https://biznetgio.creations.ren"><img src="https://img.shields.io/badge/%F0%9F%8C%90%20open%20docs-biznetgio.creations.ren-008541?style=for-the-badge" alt="Documentation site"></a>
</p>

This repository powers the docs site at [biznetgio.creations.ren](https://biznetgio.creations.ren) for two
community providers:

| Provider | Repository | Registry |
| --- | --- | --- |
| Terraform | [shirasakaren/terraform-provider-biznetgio](https://github.com/shirasakaren/terraform-provider-biznetgio) | [Terraform Registry](https://registry.terraform.io/providers/shirasakaren/biznetgio) |
| Pulumi | [shirasakaren/pulumi-biznetgio](https://github.com/shirasakaren/pulumi-biznetgio) | [Pulumi Registry](https://www.pulumi.com/registry/packages/biznetgio) |

## What's documented

- [What is Infrastructure as Code?](https://biznetgio.creations.ren/what-is-iac) - beginner friendly explainer of IaC, Terraform, and Pulumi, including how the tools actually work under the hood
- Quickstarts for [Terraform](https://biznetgio.creations.ren/quickstart) and [Pulumi](https://biznetgio.creations.ren/pulumi-quickstart)
- [Authentication](https://biznetgio.creations.ren/authentication), [package registries](https://biznetgio.creations.ren/registries), and per-resource references for both providers
- [Tutorials](https://biznetgio.creations.ren/tutorials/project-structure) - an eight-part path from project structure to a reviewed, CI-deployed production stack: project layout, environments, state and collaboration, secrets management, CI/CD, modules and components, testing and guardrails, and a full production capstone
- Guides: billing, triggers, development, and FAQ
- Full Indonesian translation of every page

## Structure

- `docs.json` - site configuration (navigation, branding, navbar)
- `index.mdx`, `what-is-iac.mdx`, `quickstart.mdx`, `pulumi-quickstart.mdx`, `authentication.mdx`, `registries.mdx` - getting started
- `terraform/` and `pulumi/` - per-provider references (installation, resources, importing)
- `tutorials/` - project structure, environments, state and collaboration, secrets, CI/CD, modules and components, testing and guardrails, and a production capstone
- `guides/` - billing, triggers, development, FAQ
- `id/` - Indonesian translation of every page

## Development

```bash
npm i -g mint     # install the Mintlify CLI
mint dev          # preview at http://localhost:3000
```

Changes pushed to the default branch deploy automatically via the Mintlify GitHub app.

## License

[Apache-2.0](LICENSE)
