# GitLab Hands-on Training Module

A hands-on Training covering self-hosted GitLab production deployment, core workflows, migration and building a profitable freelance service around GitLab.

## Prerequisites
- Linux fundamentals (CLI, SSH, package management)
- Basic networking (DNS, ports, firewalls)
- A VPS or cloud server (Ubuntu 22.04 LTS recommended, 4 vCPU / 8 GB RAM minimum)
- A registered domain name
- Upwork/Fiverr freelancer account (for Day 5)

---

## Schedule

### Day 1 — GitLab Installation on Linux Server
- GitLab editions overview (CE vs EE)
- Server sizing and OS preparation
- Install GitLab CE via official repository (apt/rpm)
- `gitlab.rb` configuration essentials (external_url, SMTP, time zone)
- Initial root password setup and first login
- Firewall rules (UFW/iptables) for ports 22, 80, 443
- **Lab:** Install GitLab CE on a fresh Ubuntu 22.04 VPS

### Day 2 — Domain, SSL & Nginx Setup
- Buying/configuring a domain (registrar, DNS A record → server IP)
- Pointing a custom domain to GitLab (`external_url` in `gitlab.rb`)
- Auto SSL via Let's Encrypt built into GitLab Omnibus
- Manual SSL option (custom cert install in `gitlab.rb`)
- Configuring Nginx as GitLab's bundled reverse proxy
- Email/SMTP configuration for notifications
- `gitlab-ctl reconfigure` and service management
- **Lab:** Secure your GitLab instance at `https://gitlab.yourdomain.com`

### Day 3 — Pushing Code & Repository Workflows
- Creating users, groups, and projects
- SSH key setup and Git remote configuration
- Cloning, branching, committing, and pushing code
- Merge requests (MR) and code review workflow
- Protected branches and approval rules
- GitLab CI/CD pipeline basics (`.gitlab-ci.yml`)
- Runners: shared vs specific, installing a GitLab Runner on Linux
- **Lab:** Push a sample project, create an MR, and run a CI pipeline

### Day 4 — Auto DevOps, Scaling & Migration
- **GitLab Auto DevOps:** enabling per project/globally, pipeline stages (build, test, security scan, deploy)
- Connecting a Kubernetes cluster or Docker host for Auto DevOps deployments
- GitLab Container Registry setup and usage
- **Migration:** importing repos from GitHub/Bitbucket/Gitea using GitLab Importer
- Migrating full GitLab instance (backup/restore with `gitlab-backup create`)
- Upgrading GitLab to a newer version safely
- Performance tuning (Puma workers, Sidekiq concurrency, PostgreSQL)
- Monitoring with GitLab's built-in Prometheus + Grafana
- **Lab:** Migrate a GitHub repo into GitLab and enable Auto DevOps

### Day 5 — Marketplace Service Development
- Identifying GitLab service niches:
  - Self-hosted GitLab setup & configuration
  - GitLab CI/CD pipeline development
  - GitHub → GitLab migration
  - GitLab Runner setup & troubleshooting
  - GitLab Auto DevOps implementation
- Writing compelling Upwork/Fiverr gig titles & descriptions
- Pricing models (fixed-price vs hourly, tiered packages)
- Portfolio/proof-of-work prep using Day 1–4 labs
- Client scoping, communication, and proposal templates
- **Lab:** Publish a live Upwork gig for GitLab services

---

## Outcomes
By the end of this Training, participants will:
- Deploy and maintain a production-grade self-hosted GitLab instance with custom domain and SSL
- Manage repositories, CI/CD pipelines, and Auto DevOps workflows
- Migrate existing projects from other Git platforms into GitLab
- Have a published, client-ready freelance service listing for GitLab

## Resources
- `/configs` — sample `gitlab.rb` configuration files
- `/scripts` — installation, backup, and migration scripts
- `/ci-templates` — reusable `.gitlab-ci.yml` templates
- `/templates` — Upwork gig and client proposal templates
- [GitLab Docs](https://docs.gitlab.com)
- [GitLab CE Downloads](https://packages.gitlab.com/gitlab/gitlab-ce)

# Disclaimer
This repository is intended to provide guidance, documentation, and support resources related to GitLab installation. Product names, trademarks, and service names belong to their respective owners.

⭐ If this repository helps you, please consider starring it and sharing it with others.
