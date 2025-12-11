# Clone All Repositories – GitHub Automation

This repository contains ready-to-use commands and scripts for cloning, listing, and backing up every repository in the GitHub account **amitsingh573**.

---

## 1. List all repositories

```bash
gh repo list amitsingh573 --limit 200 --json name,visibility,sshUrl,httpsUrl --jq '.[] | {name,visibility,sshUrl,httpsUrl}'
