# Awesome-Cryptography-Encryption

## Top Cryptography & Encryption Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Post-Quantum Readiness, Key Management & Certificate Lifecycle*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cryptography & Encryption**. These tools enable organizations to secure data at rest and in transit, manage cryptographic keys across their lifecycle, and prepare for the post-quantum transition—from cloud-managed KMS services to self-hosted PKI and PQC libraries.



**Examples** include RSA Security, Entrust, Thales CipherTrust, HashiCorp Vault, CyberArk, DigiCert, Sectigo, Keyfactor, AppViewX, and Venafi (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, post-quantum readiness, and open certificate management—ideal for security engineers, platform teams, and organizations seeking transparent, vendor-independent cryptography infrastructure.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Thales CipherTrust](https://cpl.thalesgroup.com/)**  

  **Enterprise key management and data protection platform** . Features **centralized key lifecycle**, **HSM integration**, **database encryption**, and **multi-cloud key orchestration**. **The enterprise standard** for regulated industries requiring FIPS 140-2 Level 3 validated HSMs.



- **[HashiCorp Vault (HCP)](https://www.hashicorp.com/products/vault)**  

  **Managed secrets management and PKI platform** . Features **dynamic secrets**, **transit engine for encryption-as-a-service**, **PKI secrets engine for internal CA**, and **ACME support** . **The most widely deployed secrets management platform**.



- **[CyberArk](https://www.cyberark.com/)**  

  **Privileged access management and secrets management** . Features **Conjur for machine identity**, **credential rotation**, and **centralized policy enforcement** . **The enterprise standard** for privileged access security.



- **[DigiCert](https://www.digicert.com/)**  

  **Certificate lifecycle management** with **strong PQC research track record** and **deep CA integration** . **DigiCert Trust Lifecycle Manager** provides discovery, automation, and governance. **The natural choice** for organizations using DigiCert as their primary CA.



- **[Keyfactor](https://www.keyfactor.com/)**  

  **The pragmatic enterprise CLM choice** — **Keyfactor Command** for certificate lifecycle management plus **EJBCA** for integrated PKI from one vendor . **Leads in PQC readiness** following 2025 acquisitions of InfoSec Global and CipherInsights . **EJBCA supports ML-DSA, ML-KEM, SLH-DSA, Falcon, LMS, and XMSS** with Common Criteria EAL4+ certification .



- **[Venafi (CyberArk)](https://www.venafi.com/)**  

  **Enterprise machine identity management** with the deepest Windows/Active Directory ecosystem support and proven scalability to 100K+ certificates . **TLS Protect** for certificate lifecycle management, **SSH Protect** for SSH key management. **The premium choice** for highly regulated enterprises.



- **[AppViewX](https://www.appviewx.com/)**  

  **PKI and certificate lifecycle management with strong PQC readiness** . **AVX ONE** discovers public and private trust certificates, automates provisioning and renewal, and enforces enterprise PKI policy . **PQC Assessment Tool** produces a Cryptographic Bill of Materials and a readiness score .



- **[Entrust](https://www.entrust.com/)**  

  **Enterprise certificate management** with **HSM integration** and comprehensive PKI services.



- **[Sectigo](https://www.sectigo.com/)**  

  **Enterprise certificate lifecycle management** with automated discovery, expiration monitoring, and certificate operations.



- **[RSA Security](https://www.rsa.com/)**  

  **Identity and access management** with **RSA SecurID** for MFA and **RSA Archer** for governance, risk, and compliance.



## Open-Source GitHub Projects



- **[EJBCA (Keyfactor)](https://github.com/Keyfactor/ejbca-ce)**  

  **Enterprise-grade open-source PKI certificate authority** (LGPL-2.1 dual-license with commercial enterprise edition) . **The most comprehensive open-source CA** — **supports ML-DSA, ML-KEM, SLH-DSA, Falcon, LMS, and XMSS** for post-quantum readiness with **Common Criteria EAL4+ certification** . Features **web GUI, REST API, HSM support, OCSP, and ACME** . **EJBCA is the foundation of Keyfactor's enterprise PKI offering** — the commercial edition adds advanced features and support . **The reference implementation for self-hosted certificate authority**.



- **[Step-ca (Smallstep)](https://github.com/smallstep/certificates)**  

  **Open-source certificate authority and ACME server** (Apache-2.0) . **The modern, developer-friendly CA** — **ACME support (RFC 8555)**, **short-lived certificates**, **SSH certificate authority**, and **automatic renewal** . **PQC support is experimental** via Go crypto with ML-KEM in progress . **No native certification** — depends on HSM for key protection . **Step-ca focuses on automated certificate management** for modern infrastructure . **Best for**: teams wanting a simple, automated CA for internal services.



- **[django-ca](https://github.com/mathiasertl/django-ca)**  

  **Tool to manage TLS certificate authorities and easily issue and revoke certificates** (BSD-3-Clause) . **The Django-native CA** — based on **cryptography and Django** . Features **ACMEv2, REST API, command-line, and web interface** for certificate issuance . **Certificate revocation via CRLs and OCSP** . **Private key storage on filesystem, in database, or in HSM** . **Email notifications about expiring certificates** . **Written in Python 3.11+, Django 5.2+, and cryptography 46+** . **Best for**: Django projects needing integrated CA functionality.



- **[certmesh](https://github.com/SCGIS-Wales/certmesh)**  

  **Multi-provider certificate lifecycle automation** (open-source) . **The most provider-diverse open-source CLM tool** — supports **DigiCert CertCentral, Venafi TPP, AWS ACM/ACM-PCA, Let's Encrypt/ACME** . **Certificate output to filesystem (mode 0600), Vault KV v1/v2, AWS Secrets Manager, or multiple destinations** . **Circuit breaker** for provider failures . **Prometheus Pushgateway integration** for renewal CronJob observability . **OAuth2 JWT Bearer validation with RS256 algorithm restriction** . **Best for**: multi-CA enterprise environments.



- **[Certimate](https://github.com/certimate-go/certimate)**  

  **Open-source, self-hosted SSL certificate ACME tool with visual workflow orchestration** (MIT) . **The most comprehensive open-source certificate automation platform** — **70+ domain registrars** (AWS, Cloudflare, GoDaddy, Alibaba Cloud, Tencent Cloud), **160+ deployment destinations** (Kubernetes, CDN, WAF, load balancers), **multiple ACME CAs** (Let's Encrypt, Google Trust Services, ZeroSSL, SSL.com), and **multiple notification channels** . **Zero dependencies, ~20 MB memory** — binary or Docker deployment . **The best choice for teams wanting visual workflow automation across heterogeneous infrastructure**.



- **[Certlord](https://github.com/decryptus/certlord)**  

  **TLS certificate lifecycle automation** (pre-release) . **Coordinates certificate creation and renewal through Certbot**, external PEM import, **Redis-backed HTTP challenges**, **Vault storage**, and deployment through Auton . **Optional destination TLS verification checks the certificate actually served before acknowledgement** . **StatusCake/Updown adapters optional** . **Best for**: teams wanting automated certificate renewal with verification.



- **[CIRCL (Cloudflare)](https://github.com/cloudflare/circl)**  

  **Cloudflare Interoperable, Reusable Cryptographic Library** (BSD-3-Clause) . **The most widely adopted Go cryptographic library from Cloudflare** — **supports ML-KEM modes 512/768/1024 (FIPS 203)**, **X25519MLKEM768 hybrid KEM**, **ML-DSA modes 44/65/87 (FIPS 204)**, and **SLH-DSA twelve parameter sets (FIPS 205)** . **Ongoing internal security review published in SECURITY_AUDIT.md** — findings carry CWE classification and VEX justification semantics . **Best for**: Go developers needing post-quantum cryptography with production-grade implementation.



- **[dcrypt](https://github.com/ioi-foundation/dcrypt)**  

  **Modern, high-assurance cryptographic library in Rust** (open-source) . **The first publicly released, production-ready implementation of the complete CRYSTALS-Dilithium/ML-DSA signature scheme in pure Rust with zero unsafe code, zero FFI dependencies, and full constant-time execution** . **First pure-Rust library to provide native hybrid KEM (ECDH + Kyber) and hybrid signatures (ECDSA + Dilithium) as composable primitives** . **Hybrid constructions introduce less than 10% overhead** compared to post-quantum-only implementations . **Best for**: Rust developers needing memory-safe, quantum-resistant cryptography.



- **[OpenSSL](https://github.com/openssl/openssl)**  

  **The most widely deployed cryptographic library** (Apache-2.0) . **The foundation of most TLS implementations** — **supports ML-KEM, ML-DSA, SLH-DSA, and X25519MLKEM768 hybrid group** natively since **version 3.5.0** . **The 3.5 branch is LTS, maintained until April 2030** . **Best for**: general-purpose cryptographic operations and TLS.



- **[wolfSSL](https://github.com/wolfSSL/wolfssl)**  

  **Lightweight, portable, embedded SSL/TLS library** (GPL-3.0 or commercial) . **The embedded systems standard** — **up to 19 times lower memory footprint than OpenSSL** on the same scenarios . **Two active FIPS 140-3 certificates** . **Supports ML-KEM, ML-DSA, and TLS 1.3** . **Best for**: IoT, automotive, and resource-constrained environments.



### Additional Strong Open-Source Options



- **[Vault](https://github.com/hashicorp/vault)** — Secrets management and PKI (BUSL 1.1) . **The most widely deployed open-source secrets management platform** — **dynamic secrets, transit engine, PKI secrets engine, and ACME support** . **Supports multiple auth methods (Github, tokens, certificates, cloud credentials)** . **Best for**: general-purpose secrets and key management.

- **[OpenBao](https://github.com/openbao/openbao)** — Community fork of HashiCorp Vault under MPL 2.0 (Linux Foundation) . **The open-source alternative after Vault's license change** .

- **[smallstep/cli](https://github.com/smallstep/cli)** — CLI for step-ca (Apache-2.0) . **The command-line interface for Smallstep's CA** .

- **[cert-manager](https://github.com/cert-manager/cert-manager)** — Automatically provision and manage TLS certificates in Kubernetes (Apache-2.0) . **The Kubernetes-native certificate management standard** .

- **[libsodium](https://github.com/jedisct1/libsodium)** — Modern, portable, easy-to-use crypto library (ISC) . **The standard for high-level cryptographic primitives** .

- **[Themis](https://github.com/cossacklabs/themis)** — High-level cryptographic library for storage, messaging, and session exchange (Apache-2.0) . **Cross-language support (Go, JS, Python, Ruby, Java, PHP, C++)** .

- Community **n8n** workflows for certificate expiry alerting and key rotation automation.



**Frameworks for building custom systems**: Combine **EJBCA** for self-hosted enterprise PKI with **cert-manager** for Kubernetes-native certificate automation, **CIRCL** or **dcrypt** for post-quantum cryptographic primitives, **Vault** for secrets management, and **Certimate** for multi-CA workflow orchestration—creating a fully self-hosted, enterprise-grade cryptography platform.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Cryptographic tools must follow security best practices, including HSM integration for CA private keys, audit logging for compliance, and proper key lifecycle management.

- **Open-source cryptography is mature and production-ready.** EJBCA provides **enterprise-grade PKI with Common Criteria EAL4+ certification and PQC support** . CIRCL is **Cloudflare's production cryptographic library with FIPS 203/204/205 implementations** . dcrypt is **the first pure-Rust ML-DSA implementation with zero unsafe code** . **These are genuine alternatives to commercial platforms.**

- **The post-quantum transition is the critical 2026 priority.** NIST standards (FIPS 203 ML-KEM, FIPS 204 ML-DSA, FIPS 205 SLH-DSA) are finalized . **OpenSSL 3.5+ supports ML-KEM, ML-DSA, SLH-DSA, and hybrid groups natively** . **EJBCA, CIRCL, and dcrypt already implement PQC** . **Organizations should begin PQC readiness assessments now** — the transition will take years.

- **Hybrid mode is the recommended transition path.** **Activate hybrid rather than pure post-quantum** — if an unexpected weakness is discovered in ML-KEM or ML-DSA, the classical component (X25519 or ECDSA) continues to protect the connection . **This is the best practice recommended by OpenSSL and Cloudflare** .

- **Open-source key management systems have clear trade-offs.** **HashiCorp Vault** is the most feature-rich with multiple auth methods and HSM support . **OpenStack Barbican** is OpenStack-specific with limited external utility . **Lyft Confidant** integrates deeply with AWS KMS . **CyberArk Conjur** is versatile but complex to configure . **Choose based on your deployment environment and operational capacity** .

- **Self-hosted open-source solutions require proper HSM integration, key lifecycle management, and ongoing maintenance.** **CA private keys are the root of trust** — compromise undermines every certificate issued. **HSM integration is non-negotiable for production PKI** .



---



**Made for security engineers, platform teams, and organizations building transparent cryptography solutions.**  

Let's make Cryptography & Encryption more open, data-driven, and post-quantum ready.
