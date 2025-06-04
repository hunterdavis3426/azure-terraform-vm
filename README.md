## Overview

This project uses Terraform to deploy an Ubuntu VM in Azure, automatically install Docker, and run a Ghost CMS instance behind an NGINX reverse proxy. It integrates with DuckDNS for dynamic DNS and uses Let's Encrypt to secure the site with HTTPS.

## Features

- Infrastructure-as-Code via Terraform
- Azure VM provisioning
- Docker container for Ghost CMS (shifted to nginx hosting)
- NGINX reverse proxy
- HTTPS via Let's Encrypt (Certbot)
- DuckDNS for domain management

## Prerequisites

- Azure account
- Terraform
- Docker installed if hosting via container (locally or via cloud-init)
- domain for HTTPS

## Deployment Steps

1. Clone repo
2. Set variables and update main.tf + variables.tf with azure resource group, VM specs/size, credentials, and your DNS token
3. Deploy w/ terraform
4. ssh into VM
5. Set up nginx + SSL with Certbot


