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
- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saashosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global Managed DNS and Cloud Network Infrastructure market is valued at approximately **$2.1 billion in 2026** (expanding within a broader **$16+ billion** enterprise DDI market) and growing at an ~18–22% CAGR driven by edge compute, Anycast routing, and Zero Trust security. The sector is **moderately concentrated to oligopolistic** at the hyperscale edge—dominated by a handful of mega-cap cloud providers (AWS, Microsoft, Google) and specialized edge/CDN titans (Cloudflare, Akamai)—while remaining fragmented across niche enterprise traffic management, hybrid private DDI appliances, and open-source self-hosted implementations.

## SaaS/Hosted Platforms

| Product | Company Size (Valuation / Market Cap) | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|---------------------------------------|-------------|-------------------|--------------------------|
| **[Azure DNS](https://azure.microsoft.com/en-us/products/dns/)** | ~$4.04 Trillion (Microsoft Market Cap) | Public and private DNS zone hosting with Azure integration, alias records, and Traffic Manager. | $0.50/hosted zone/mo (first 25); $0.40/million queries (first 1B) | **Free trial**: 30-day free trial with $200 credit applicable to Azure DNS zones and queries (no permanent free tier) |
| **[Google Cloud DNS](https://cloud.google.com/dns)** | ~$3.54 Trillion (Alphabet Market Cap) | Global Anycast authoritative DNS with 100% SLA, private zones, DNS forwarding, and DNSSEC. | $0.20/managed zone/mo (first 25); $0.40/million queries (first 1B) | **Free trial**: 90-day free trial with $300 cloud credits usable across GCP services (no permanent free tier for Cloud DNS) |
| **[AWS Route 53](https://aws.amazon.com/route53/)** | ~$2.89 Trillion (Amazon Market Cap) | Highly available authoritative DNS with health checks, latency routing, geolocation, and failover. | $0.50/hosted zone/mo (first 25); $0.40/million queries (first 1B) | **Free trial & resource limits**: No free hosted zones; free alias queries mapped to AWS resources (CloudFront/ALB), up to 1,000 CIDR blocks/mo & 50 AWS endpoint health checks |
| **[Oracle Dyn (OCI DNS)](https://www.oracle.com/cloud/networking/dns/)** | ~$350 Billion (Oracle Market Cap) | Enterprise managed DNS and traffic steering natively hosted on Oracle Cloud Infrastructure. | $0.85/million queries (no base monthly zone fee) | **Free forever**: Oracle Cloud Always Free includes up to 5 public DNS zones with 25,000 records per zone |
| **[NS1 Connect (IBM)](https://www.ibm.com/products/ns1-connect)** | ~$230 Billion (IBM Market Cap) | Developer & DevOps-centric enterprise DNS with advanced traffic steering filter chains and real-time telemetry. | Essentials plan starts at $99/mo (includes up to 30M queries and 1,000 records) | **Free forever & 30-day trial**: 30-day free enterprise trial (50M queries, 500 records); defaults to Free Developer Tier forever (5M queries/mo, 500 records, 1 filter chain, 2 monitors) |
| **[Cloudflare](https://www.cloudflare.com/)** | ~$100 Billion (Cloudflare Market Cap) | Global edge network with authoritative DNS, DDoS protection, CDN, and Workers serverless compute. | Free: $0/mo; Pro: $25/mo; Business: $200/mo | **Free forever**: unmetered DDoS mitigation, authoritative DNS, global CDN, 100k Workers requests/day |
| **[Zoho Domains](https://www.zoho.com/domains/)** | ~$13.5 Billion (Zoho Valuation) | Transparent domain registration and integrated DNS hosting with zero hidden renewal markups. | Free DNS hosting with registered domain (domains start at $11.99/year for .com with free WHOIS privacy) | **Free forever**: Complete DNS zone management (A, CNAME, MX, TXT, SRV records) included free indefinitely with any domain |
| **[Akamai Edge DNS](https://www.akamai.com/products/edge-dns)** | ~$12.5 Billion (Akamai Market Cap) | Highly resilient Anycast DNS built on the distributed Akamai platform with zone-based pricing and DDoS absorption. | Zone-based flat annual/monthly pricing (query-independent fixed fee structure) | **Free trial**: Enterprise trial evaluation available upon request through sales & Akamai Control Center Marketplace |
| **[Neustar UltraDNS (Vercara / DigiCert)](https://vercara.com/ultradns)** | ~$8.0+ Billion (DigiCert Valuation) | Carrier-grade authoritative DNS with 100% uptime SLA, global traffic management, and multi-Tbps DDoS mitigation. | Starts at ~$49/mo (standard self-serve baseline); custom enterprise contracts | **Free trial**: 30-day guided enterprise proof-of-concept / evaluation via DigiCert/Vercara sales |
| **[Fastly](https://www.fastly.com/)** | ~$3.0 Billion (Fastly Market Cap) | High-performance secondary DNS integrated into Fastly's edge cloud and modern CDN architecture. | Secondary DNS billed per 1M responses (requires active delivery contract) | **Free trial / recurring credit**: Recurring $50 monthly developer usage credit to test edge delivery and compute resources |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Pi-hole](https://github.com/pi-hole/pi-hole)** | [![Stars](https://img.shields.io/github/stars/pi-hole/pi-hole?style=social&color=white)](https://github.com/pi-hole/pi-hole/stargazers) | Network-wide ad blocking and private sinkhole DNS server providing local caching, DHCP, and privacy-focused DNS control. |
| **[AdGuard Home](https://github.com/AdguardTeam/AdGuardHome)** | [![Stars](https://img.shields.io/github/stars/AdguardTeam/AdGuardHome?style=social&color=white)](https://github.com/AdguardTeam/AdGuardHome/stargazers) | Network-wide ads, trackers, and malware-blocking DNS server with native support for DNS-over-HTTPS (DoH), DNS-over-TLS (DoT), and DNS-over-QUIC (DoQ). |
| **[CoreDNS](https://github.com/coredns/coredns)** | [![Stars](https://img.shields.io/github/stars/coredns/coredns?style=social&color=white)](https://github.com/coredns/coredns/stargazers) | Cloud-native DNS server (CNCF graduated) designed for Kubernetes service discovery with a fast, plugin-based architecture. |
| **[miekg/dns](https://github.com/miekg/dns)** | [![Stars](https://img.shields.io/github/stars/miekg/dns?style=social&color=white)](https://github.com/miekg/dns/stargazers) | High-performance, idiomatic Go DNS library used as the foundational engine behind CoreDNS, Kubernetes DNS, and microservice discovery frameworks. |
| **[Unbound](https://github.com/NLnetLabs/unbound)** | [![Stars](https://img.shields.io/github/stars/NLnetLabs/unbound?style=social&color=white)](https://github.com/NLnetLabs/unbound/stargazers) | High-performance validating, recursive, and caching DNS resolver with built-in DNSSEC and DNS-over-TLS support. |
| **[PowerDNS](https://github.com/PowerDNS/pdns)** | [![Stars](https://img.shields.io/github/stars/PowerDNS/pdns?style=social&color=white)](https://github.com/PowerDNS/pdns/stargazers) | Robust authoritative DNS server with flexible database backends (SQL, LDAP), automated DNSSEC signing, and dnsdist load balancer. |
| **[DNSControl](https://github.com/StackExchange/dnscontrol)** | [![Stars](https://img.shields.io/github/stars/StackExchange/dnscontrol?style=social&color=white)](https://github.com/StackExchange/dnscontrol/stargazers) | Infrastructure-as-code (IaC) system for managing DNS zones across dozens of DNS service providers and BIND zonefiles simultaneously. |
| **[octoDNS](https://github.com/octodns/octodns)** | [![Stars](https://img.shields.io/github/stars/octodns/octodns?style=social&color=white)](https://github.com/octodns/octodns/stargazers) | GitOps-driven multi-provider DNS configuration management and synchronization tool for configuring multi-cloud and redundant DNS setups. |
| **[BIND 9](https://github.com/isc-projects/bind9)** | [![Stars](https://img.shields.io/github/stars/isc-projects/bind9?style=social&color=white)](https://github.com/isc-projects/bind9/stargazers) | The reference implementation of authoritative and recursive DNS. Supports DNSSEC, TSIG, views, and zone transfers. |
| **[NSD](https://github.com/NLnetLabs/nsd)** | [![Stars](https://img.shields.io/github/stars/NLnetLabs/nsd?style=social&color=white)](https://github.com/NLnetLabs/nsd/stargazers) | High-speed, authoritative-only RFC-compliant DNS name server designed for root servers and top-level domain registries. |
| **[Knot Resolver](https://github.com/CZ-NIC/knot-resolver)** | [![Stars](https://img.shields.io/github/stars/CZ-NIC/knot-resolver?style=social&color=white)](https://github.com/CZ-NIC/knot-resolver/stargazers) | Modular, extensible caching full DNS resolver implementing modern RFC standards, DNS-over-TLS, and Lua scripting. |
| **[Knot DNS](https://github.com/CZ-NIC/knot)** | [![Stars](https://img.shields.io/github/stars/CZ-NIC/knot?style=social&color=white)](https://github.com/CZ-NIC/knot/stargazers) | High-performance authoritative-only DNS server with automated DNSSEC signing, on-the-fly zone updates, and geographic balancing. |

**Frameworks for building custom systems**: Combine **PowerDNS** or **BIND 9** for authoritative serving, **Unbound** or **Knot Resolver** for recursive resolution and DNSSEC validation, **CoreDNS** for Kubernetes-native service discovery, and **DNSControl** or **octoDNS** for multi-cloud GitOps DNS synchronization—creating a fully resilient DNS infrastructure stack without per-query billing.

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
