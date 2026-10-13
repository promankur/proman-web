# Proman 2.0 — Official Website

> **45+ Years of Shaping Pharma Success**  
> *Brand Story • PMT Alignment • Assets that Convert*  
> Founder & Managing Partner: **Ankur Gupta** (BITS Pilani · IIM Ahmedabad)  
> Domains: [`promankur.com`](https://www.promankur.com) · [`www.promankur.com`](https://www.promankur.com)

---

## Migration History (October 2026)

This repository holds the high-performance static release of **Proman 2.0**, migrated away from Wix to a modern, zero-maintenance static architecture hosted on **Vercel** and managed via **Cloudflare**.

### Why the Migration Was Done
1. **Eliminated Recurring Wix Subscriptions**: Avoided ongoing annual renewal costs for a static informational and portfolio site.
2. **Speed & Performance**: Replaced Wix’s ~750 KB JavaScript bundle and heavy background bloat with clean, semantic HTML5/CSS3 that loads across global edge locations in milliseconds.
3. **Infrastructure Consolidation**: Brought `promankur.com` onto the exact same modern stack powering [`vishnu.promankur.com`](https://vishnu.promankur.com) (Vercel + Cloudflare).
4. **Complete Data & Asset Preservation**:
   - Extracted 100% of the original master visuals in pristine quality:
     - `proman_logo.png` — High-resolution 2025 Proman 2.0 identity
     - `hero_bg.webp` — Header pharma strategy artwork
     - `chaos_to_precision.jpg` — PALLP Chaos-to-Precision architecture
     - `clients_alliances.png` — Clients & Alliances network diagram
     - `ankur_profile.jpg` — Founder portrait
   - Preserved all core messaging, including:
     - **3 Pillars**: Clarity $\rightarrow$ Alignment $\rightarrow$ Speed
     - **3-Stage Approach**: Diagnose $\rightarrow$ Design $\rightarrow$ Deliver
     - **Client Value**: Sharper messaging, campaign readiness, field clarity
     - **Founder Profile**: 45+ years track record, 1000+ projects delivered
     - **Contact & Channels**: Direct call (`+91 9324726587`), email (`promankur@gmail.com`), Mumbai office, and social links.

---

## File Structure

```text
proman-web/
├── assets/
│   ├── ankur_profile.jpg         # Founder portrait
│   ├── chaos_to_precision.jpg    # Methodology infographic
│   ├── clients_alliances.png     # Clients and alliances network
│   ├── hero_bg.webp              # Hero section visual
│   ├── hero_bg_mobile.webp       # Mobile responsive hero visual
│   └── proman_logo.png           # Master Proman 2.0 identity
├── coming.html                   # "Ankur Gupta: Thinker • Creator • Builder"
├── index.html                    # Proman 2.0 main landing page
├── privacy-policy.html           # 6-point clear privacy policy
├── vercel.json                   # Clean URLs configuration
└── README.md                     # Documentation & migration record
```

---

## Infrastructure & Routing

| Layer | Provider | Configuration |
| :--- | :--- | :--- |
| **Domain Registrar** | PublicDomainRegistry | Managed under Proman account |
| **DNS Management** | **Cloudflare** | Nameservers: `tony.ns.cloudflare.com` / `grace.ns.cloudflare.com` |
| **Web Hosting** | **Vercel** | Git continuous deployment from `promankur/proman-web` |
| **Email Routing** | **Cloudflare Email Routing** | Directs incoming mail to `promankur@gmail.com` |

### DNS Record Setup for Vercel
In Cloudflare DNS for `promankur.com`:
- **`@` (Apex domain)** &rarr; `A` record pointing to `76.76.21.21` (or CNAME `cname.vercel-dns.com` with CNAME flattening)
- **`www`** &rarr; `CNAME` record pointing to `cname.vercel-dns.com`
- **`vishnu`** &rarr; `CNAME` pointing to Vercel (`promankur/Vishnu`)

---

## Local Development & Edits

Because this site uses pure modern HTML5, CSS, and minimal vanilla JavaScript with clean URLs:
* No npm install, bundler, or build step is required.
* Simply open `index.html` in any browser to preview changes.
* Any git commit pushed to `main` automatically deploys live to Vercel within seconds.
