# ALU Web Stack

This repository contains projects for configuring a load-balanced web infrastructure with DNS subdomains and HTTPS/SSL, built as part of the ALU System Engineering & DevOps track.

## Project: HTTPS/SSL and DNS Subdomains

Located in the `https_ssl/` directory.

### What this project does

- Configures DNS A records so that the following subdomains resolve to the correct servers:
  - `www` → points to `lb-01` (the load balancer)
  - `lb-01` → points to `lb-01`
  - `web-01` → points to `web-01`
  - `web-02` → points to `web-02`
- Includes a Bash script, `0-world_wide_web`, that uses `dig` and `awk` to look up and display DNS record information for these subdomains.

### Usage

Display info for all four default subdomains:
```bash
./0-world_wide_web <domain>
```

Display info for a single specific subdomain:
```bash
./0-world_wide_web <domain> <subdomain>
```

### Example output

The subdomain www is a A record and points to <ip>
The subdomain lb-01 is a A record and points to <ip>
The subdomain web-01 is a A record and points to <ip>
The subdomain web-02 is a A record and points to <ip>
