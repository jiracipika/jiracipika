<div align="center">

# @jiracipika

**Cloud infrastructure engineer · Azure · Terraform · secure-by-default IaC**

</div>

Systems background (Darwin/XNU kernel & platform work — see pinned repos), now
building production-grade Azure infrastructure as code.

## Azure Cloud Engineering Portfolio

Ten repositories, one standard: runnable Terraform modules, security controls,
unit-tested policy, and an **honest validation log** in every repo —
`docs/VALIDATION.md` records the real commands, real timestamps, the failures
that broke validation, and the schema-verified fixes. No stock console
screenshots.

Everything is **offline-validated and deploy-gated** (`deploy_enabled = false`
by default): `terraform plan` with defaults proposes zero resources, and
nothing touches a paid subscription without explicit owner review.

| Repository | What it demonstrates |
|---|---|
| [azure-secure-static-website](https://github.com/jiracipika/azure-secure-static-website) | Front Door Premium + WAF (Prevention) + Private Link to a hardened storage origin (Entra-only auth), GitHub OIDC deploy identity, accessible demo site — **[live demo](https://jiracipika.github.io/azure-secure-static-website/)** |
| [azure-landing-zone](https://github.com/jiracipika/azure-landing-zone) | 9-node management-group hierarchy, governance baseline (allowed-locations Deny, VM-SKU Deny, tag Audit, diagnostics DeployIfNotExists), least-privilege custom role, hub-spoke with Azure Firewall + Bastion, budget alerts — 64 tests + a policy simulator that parses the real HCL |
| [azure-terraform-cicd](https://github.com/jiracipika/azure-terraform-cicd) | OIDC-federated plan/apply identities, promotion policy as code, inert environment-gated pipeline templates, validation-only CI — 70-test battery + pipeline policy simulator |
| [azure-monitoring-cost-control](https://github.com/jiracipika/azure-monitoring-cost-control) | Log Analytics with cost brakes (ingestion quota, retention), KQL alert rules, 50/80/100% budgets, triage workbook — monitor simulator replaying alert/budget state machines against the real HCL |
| 6 more | networking, HA webapp, disaster recovery, hybrid hub-spoke, identity & access, production AKS — advancing one milestone every week |

## Currently

- Open to freelance Azure/Terraform infrastructure work: secure static sites,
  landing zones, CI/CD pipelines with OIDC (no stored secrets),
  monitoring & cost guardrails.
- Contact: *(to be added)*

> Every repo documents its own teardown path and cost estimate before anything
> is ever deployed. Infrastructure you can audit before you pay for it.
