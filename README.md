# Awesome-Cloud-Network-DNS-Infrastructure

## Top Cloud Network & DNS Infrastructure Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Authoritative DNS, Global Traffic Management & Edge Network Services*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Network & DNS Infrastructure**. These tools provide the foundational layer for internet routing—covering authoritative DNS hosting, global server load balancing (GSLB), DNSSEC, DDoS-protected resolution, and edge compute that integrates with DNS-level traffic steering.

**Examples** include Cloudflare, AWS Route 53, Google Cloud DNS, Azure DNS, NS1 (IBM), Akamai Edge DNS, Fastly, Oracle Dyn, Neustar UltraDNS, and Zoho Domains (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted authoritative DNS servers, DNS control planes, and recursive resolvers—ideal for network engineers, SREs, and organizations seeking transparent, vendor-neutral DNS infrastructure without per-query billing surprises.

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Cloudflare](https://www.cloudflare.com/)** | Global edge network with authoritative DNS, DDoS protection, CDN, and Workers serverless compute. DNS is bundled into all plans; the free plan includes unmetered DDoS protection and basic DNS . | Free: $0; Pro: $25/month; Business: $200/month; Enterprise: custom  | **Free forever**: unmetered DDoS protection, authoritative DNS, global CDN, unlimited bandwidth (fair use), 100k Workers requests/day . |
| **[AWS Route 53](https://aws.amazon.com/route53/)** | Highly available authoritative DNS with health checks, latency-based routing, geolocation, and failover policies. Integrates with AWS resources via alias records (free queries for ELB/CloudFront aliases) . | Hosted zone: ~€0.50/month (first 25 zones); queries: €0.40/million (first 1B), €0.20/million thereafter (EU pricing) [citation:2] | **No free tier** for hosted zones; queries to alias records mapped to AWS resources are free [citation:2]. |
| **[Google Cloud DNS](https://cloud.google.com/dns)** | Authoritative DNS with 100% SLA, global anycast, private zones, DNS forwarding, and DNSSEC. Integrates with GCP services and supports DNS-based traffic management . | Managed zone: $0.20/month (first 25); queries: $0.40/million (first 1B), $0.20/million thereafter [citation:3][citation:15] | **No free tier** for Cloud DNS [citation:3]. |
| **[Azure DNS](https://azure.microsoft.com/en-us/products/dns/)** | Hosting for public and private DNS zones with Azure integration, alias records, and traffic manager for GSLB. Private resolver available for hybrid DNS . | Hosted zone: ~¥3.98/month (first 25 zones); queries: ~¥4.07/million (China pricing) [citation:4] | **No free tier**; Azure free account credits may apply. |
| **[NS1 Connect (IBM)](https://www.ibm.com/products/ns1-connect)** | Enterprise DNS with advanced traffic steering (filter chains), real-time monitoring, spike protection, and 100% uptime SLA. Acquired by IBM; strong for API-driven and DevOps-centric DNS workflows . | Quote-only (contact sales for pricing) [citation:5] | **No free tier**; trial via sales. |
| **[Akamai Edge DNS](https://www.akamai.com/products/edge-dns)** | Enterprise authoritative DNS built on the Akamai edge network with global anycast, DDoS mitigation, and integration with Akamai's CDN and security products. | Custom pricing (quote-only); professional services/onboarding $10k–$50k+ reported [citation:6] | **No free tier**; trial via sales. |
| **[Fastly](https://www.fastly.com/)** | Edge cloud platform with DNS capabilities (via Fastly DNS) integrated with CDN and Compute@Edge. Usage-based pricing with volume discounts; positioned for performance-conscious teams . | Quote-only (usage-based with volume discounts) [citation:7] | **Free trial**: $50 credit for new accounts. |
| **[Oracle Dyn](https://dyn.com/)** | Managed DNS and traffic management (acquired by Oracle). Dyn's consumer Dynamic DNS service is priced separately from enterprise DNS. | Enterprise DNS: quote-only; DynDNS consumer: $55/year [citation:8] | **No free tier** for enterprise DNS; DynDNS consumer paid only. |
| **[Neustar UltraDNS](https://www.home.neustar/)** | Enterprise DNS with 100% uptime SLA, DDoS protection, and advanced traffic management. Widely used in financial services and healthcare. | From ~$49/month (third-party listing) [citation:9] | **No free tier**; trial via sales. |
| **[Zoho Domains](https://www.zoho.com/domains/)** | Domain registration and DNS management within the Zoho ecosystem. Positioned as straightforward and predictable without aggressive promotional pricing . | Quote via Zoho Domains | No published free tier; Zoho ecosystem bundles may apply. |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[BIND 9](https://github.com/isc-projects/bind9)** | [![Stars](https://img.shields.io/github/stars/isc-projects/bind9?style=social&color=white)](https://github.com/isc-projects/bind9/stargazers) | The reference implementation of authoritative and recursive DNS. Supports DNSSEC, TSIG, views, and zone transfers. The foundation of most internet DNS infrastructure. |
| **[PowerDNS](https://github.com/PowerDNS/pdns)** | [![Stars](https://img.shields.io/github/stars/PowerDNS/pdns?style=social&color=white)](https://github.com/PowerDNS/pdns/stargazers) | Authoritative DNS server with multiple backends (SQL, LDAP, files) and a separate recursive resolver. Includes DNSSEC signing and geographic balancing capabilities . |
| **[CoreDNS](https://github.com/coredns/coredns)** | [![Stars](https://img.shields.io/github/stars/coredns/coredns?style=social&color=white)](https://github.com/coredns/coredns/stargazers) | Cloud-native DNS server (CNCF graduated) designed for Kubernetes service discovery. Plugin-based architecture, supports DNS over TLS/HTTPS . |
| **[Unbound](https://github.com/NLnetLabs/unbound)** | [![Stars](https://img.shields.io/github/stars/NLnetLabs/unbound?style=social&color=white)](https://github.com/NLnetLabs/unbound/stargazers) | Validating, recursive, and caching DNS resolver with DNSSEC support. Can also serve as an authoritative server for small zones; supports DNS over TLS . |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Knot DNS](https://github.com/CZ-NIC/knot)** | [![Stars](https://img.shields.io/github/stars/CZ-NIC/knot?style=social&color=white)](https://github.com/CZ-NIC/knot/stargazers) | High-performance authoritative DNS server with DNSSEC signing and geographic balancing . |
| **[NSD](https://github.com/NLnetLabs/nsd)** | [![Stars](https://img.shields.io/github/stars/NLnetLabs/nsd?style=social&color=white)](https://github.com/NLnetLabs/nsd/stargazers) | Authoritative-only DNS server with DNSSEC signing; lightweight and secure . |
| **[ZoneForge](https://github.com/zoneforge/zoneforge)** | [![Stars](https://img.shields.io/github/stars/zoneforge/zoneforge?style=social&color=white)](https://github.com/zoneforge/zoneforge/stargazers) | Go + HTMX DNS administration control plane for PowerDNS and BIND9. Single-binary deployment, focused on safe DNS operations [citation:12]. |

**Frameworks for building custom systems**: Combine **PowerDNS** or **BIND 9** for authoritative serving, **Unbound** for recursive resolution and DNSSEC validation, **CoreDNS** for Kubernetes-native service discovery, and **ZoneForge** for a lightweight management UI—creating a fully self-hosted DNS infrastructure stack without per-query billing.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- DNS infrastructure is a critical security boundary; enforce DNSSEC where possible, restrict zone transfer (AXFR/IXFR) to authorized secondaries, and monitor for DNS hijacking or cache poisoning.
- Self-hosted DNS servers require proper anycast or redundant deployment, DDoS mitigation, and regular security updates; a single authoritative server is a single point of failure.

---

**Made for network engineers, SREs, platform teams, and organizations building resilient DNS infrastructure.**  
Let's make cloud DNS and network services more open, observable, and resilient.
