# Day 13 — Managing Sensitive Data

This folder is a **placeholder** so Day 13 appears alongside the other numbered challenge folders.

## Curriculum (Day 13)

- Secret leak paths: `.tf` files, variable defaults, **plaintext state**  
- AWS Secrets Manager + `data` sources (no passwords in Git)  
- `sensitive = true` on variables and outputs  
- Remote state: encryption, bucket policy, no public access

## Where to implement in this workspace

| Topic | Location |
|--------|----------|
| Remote state encryption + `prevent_destroy` | `terraform-challenge-day16/modules/terraform-state/` |
| `.gitignore` for state / `.terraform` / `*.tfvars` | Each repo’s `.gitignore` + workspace root `.gitignore` |
| Provider auth via env / `aws configure` | Days 1–2 (no code); never commit keys |

## Free tier

Secrets Manager has a **free trial** period; for labs, prefer **mock** secrets or delete secrets after use.

---

Add a small root module here (`main.tf`, `versions.tf`) if you want a dedicated Day 13 repo that only creates a secret + reads it — optional.
