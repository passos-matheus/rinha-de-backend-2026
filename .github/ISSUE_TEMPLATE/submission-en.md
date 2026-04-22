---
name: Submission (EN)
about: Open a submission for Rinha de Backend 2026. The engine runs the tests automatically.
title: "[SUBMISSION] "
labels: ["submission"]
assignees: []
---

> This template is for **submissions**. To report a bug, ask a question or share a suggestion, go back and pick **Open a blank issue**.

## Required checklist

Before opening the issue, confirm:

**Resources and network**
- [ ] My submission respects the limit of **1 CPU unit** and **350MB of memory**, across all services declared in `docker-compose.yml`.
- [ ] My backend listens on **port 9999**.
- [ ] The images used are compatible with **linux/amd64**.
- [ ] Network mode is set to **bridge** (`host` mode is not allowed).
- [ ] No service runs in **privileged** mode.

**Topology**
- [ ] I have **at least one load balancer** and **two API instances**.
- [ ] My load balancer complies with the Gabriel-2025 law: it has no application logic and does not respond on behalf of the APIs (no `~smart~ load balancing`).

**Repository and submission**
- [ ] My repository is **public**.
- [ ] The repository has a `main` branch with the source code and a `submission` branch with the execution files.
- [ ] The `submission` branch has `docker-compose.yml` at the **root**.
- [ ] The `submission` branch has a filled-in `info.json`.
- [ ] I have opened (or already merged) a PR adding my participant file at `./participants/<my-github-username>.json`.

## Test execution

The Rinha engine scans issues whose description contains `rinha/test` and runs the tests automatically. **Do not remove the line below.** If you have more than one submission, also provide the `id` — for example, `rinha/test ana-experimental`.

```
rinha/test
```

---

Have fun! 🚀
