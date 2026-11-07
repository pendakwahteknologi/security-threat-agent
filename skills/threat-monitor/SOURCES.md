# Threat Monitor Sources

Starting configuration from Pendakwah Teknologi `security-threat-agent` (CC-BY-4.0), tested 2026-11-07 (108/112 reachable).

Prefer APIs / JSON / RSS / CSAF / VEX over page scraping. Documentation URLs are integration guides, not event feeds. Record auth needs, freshness, and failures per run. Never silently swap a primary source for a mirror.

Known-blocked without browser/account (2026-11-07): Australian cyber alerts (timeout from MY), Broadcom/VMware portal (bot check), SentinelLABS (bot check), Wordfence DB (bot challenge).

## A. Core vuln + exploitation

- CISA KEV catalog: https://www.cisa.gov/known-exploited-vulnerabilities-catalog
- CISA KEV JSON: https://www.cisa.gov/sites/default/files/feeds/known_exploited_vulnerabilities.json
- CISA KEV repo: https://github.com/cisagov/kev-data
- CVE List V5: https://github.com/CVEProject/cvelistV5
- CISA Vulnrichment: https://github.com/cisagov/vulnrichment
- NIST NVD: https://nvd.nist.gov/
- NVD API docs: https://nvd.nist.gov/developers/vulnerabilities
- NVD bulk feeds: https://nvd.nist.gov/vuln/data-feeds
- FIRST EPSS: https://www.first.org/epss/
- EPSS data docs: https://www.first.org/epss/data
- EPSS API docs: https://api.first.org/epss/
- EPSS JSON API: https://api.first.org/data/v1/epss
- EPSS daily CSV: https://epss.empiricalsecurity.com/epss_scores-current.csv.gz
- GitHub Advisories: https://github.com/advisories
- GitHub Advisory DB: https://github.com/github/advisory-database
- GitHub Advisory API docs: https://docs.github.com/en/rest/security-advisories/global-advisories
- OSV: https://osv.dev/
- OSV API docs: https://google.github.io/osv.dev/api/
- VulnCheck KEV docs: https://docs.vulncheck.com/community/vulncheck-kev
- VulnCheck KEV schema: https://docs.vulncheck.com/community/vulncheck-kev/schema
- ENISA EUVD: https://euvd.enisa.europa.eu/

## B. CERT advisories (incl. Malaysia)

- MyCERT: https://www.mycert.org.my/
- CyberSecurity Malaysia: https://www.cybersecurity.my/portal-main/advisories
- NACSA: https://www.nacsa.gov.my/alert.php
- NC4: https://www.nc4.gov.my/alertAdvisory?lang=en
- CISA advisories: https://www.cisa.gov/news-events/cybersecurity-advisories
- CISA ICS advisories: https://www.cisa.gov/news-events/ics-advisories
- CERT/CC notes: https://kb.cert.org/vuls/
- CERT-EU: https://cert.europa.eu/publications/security-advisories/
- CERT-FR: https://cert.cyber.gouv.fr/
- UK NCSC threat reports: https://www.ncsc.gov.uk/section/keep-up-to-date/threat-reports
- Australian alerts: https://www.cyber.gov.au/alerts-and-advisories
- Singapore CSA: https://www.csa.gov.sg/alerts-and-advisories/
- JPCERT/CC: https://www.jpcert.or.jp/english/

## C. Vendor advisories

- Microsoft Update Guide: https://msrc.microsoft.com/update-guide/
- Microsoft CSAF/VEX: https://msrc.microsoft.com/csaf
- Cisco: https://sec.cloudapps.cisco.com/security/center/publicationListing.x
- Fortinet PSIRT: https://www.fortiguard.com/psirt
- Palo Alto: https://security.paloaltonetworks.com/
- SonicWall PSIRT: https://psirt.global.sonicwall.com/
- Citrix: https://support.citrix.com/securitybulletins
- Ivanti RSS: https://www.ivanti.com/blog/topics/security-advisory/rss
- F5: https://my.f5.com/manage/s/new-updated-articles
- Broadcom/VMware: https://support.broadcom.com/
- Oracle: https://www.oracle.com/security-alerts/
- SAP: https://support.sap.com/en/my-support/knowledge-base/security-notes-news.html
- Atlassian: https://www.atlassian.com/trust/security/advisories
- Dell: https://www.dell.com/support/security/en-my
- Siemens ProductCERT: https://cert-portal.siemens.com/
- AWS: https://aws.amazon.com/security/security-bulletins/
- Google Cloud: https://docs.cloud.google.com/support/bulletins
- Red Hat: https://access.redhat.com/security/security-updates/security-advisories
- Ubuntu: https://ubuntu.com/security/notices
- Debian: https://www.debian.org/security/
- SUSE: https://www.suse.com/support/update/
- Apple: https://support.apple.com/en-us/100100
- Android: https://source.android.com/docs/security/bulletin
- Chrome releases: https://chromereleases.googleblog.com/
- Mozilla: https://www.mozilla.org/en-US/security/advisories/

## D. Early disclosure / research

- Google Project Zero: https://projectzero.google/
- watchTowr Labs: https://labs.watchtowr.com/
- Searchlight/Assetnote: https://www.slcyber.io/research
- ZDI published: https://www.zerodayinitiative.com/advisories/published/
- Horizon3: https://horizon3.ai/attack-research/
- Rapid7: https://www.rapid7.com/blog/
- Tenable: https://www.tenable.com/research
- VulnCheck: https://www.vulncheck.com/blog
- GreyNoise research: https://www.greynoise.io/blog
- GreyNoise intel docs: https://docs.greynoise.io/docs/vulnerability-prioritization-overview
- PortSwigger: https://portswigger.net/research
- oss-security: https://www.openwall.com/lists/oss-security/
- Full Disclosure: https://seclists.org/fulldisclosure/

## E. Threat intel / incident research

- Google/Mandiant: https://cloud.google.com/blog/topics/threat-intelligence
- Microsoft intel: https://www.microsoft.com/en-us/security/blog/topic/threat-intelligence/
- Cisco Talos: https://blog.talosintelligence.com/
- Unit 42: https://unit42.paloaltonetworks.com/
- CrowdStrike: https://www.crowdstrike.com/en-us/blog/
- SentinelLABS: https://www.sentinelone.com/labs/
- Elastic: https://www.elastic.co/security-labs
- Kaspersky Securelist: https://securelist.com/
- ESET: https://www.welivesecurity.com/en/
- Trend Micro: https://www.trendmicro.com/en_us/research.html
- Wiz: https://www.wiz.io/blog
- Aqua: https://www.aquasec.com/blog/
- SANS ISC: https://isc.sans.edu/

## F. Supply chain / malicious packages

- OpenSSF malicious-packages: https://github.com/ossf/malicious-packages
- Socket: https://socket.dev/blog
- ReversingLabs: https://www.reversinglabs.com/blog
- Sonatype: https://www.sonatype.com/blog
- Snyk DB: https://security.snyk.io/
- PyPA DB: https://github.com/pypa/advisory-database
- RustSec: https://rustsec.org/
- Go vuln DB: https://vuln.go.dev/
- Wordfence: https://www.wordfence.com/threat-intel/vulnerabilities
- Patchstack: https://patchstack.com/database/

## G. Infra / dev tools

- Kubernetes CVE feed: https://kubernetes.io/docs/reference/issues-security/official-cve-feed/
- Jenkins: https://www.jenkins.io/security/advisories/
- OpenSSL: https://openssl-library.org/news/vulnerabilities/index.html
- Apache httpd: https://httpd.apache.org/security/vulnerabilities_24.html
- NGINX: https://nginx.org/en/security_advisories.html
- Node.js: https://nodejs.org/en/blog/vulnerability
- PHP: https://www.php.net/releases/

## H. IOCs / malicious infra

- URLhaus: https://urlhaus.abuse.ch/
- ThreatFox: https://threatfox.abuse.ch/
- MalwareBazaar: https://bazaar.abuse.ch/
- Feodo: https://feodotracker.abuse.ch/
- Shadowserver: https://www.shadowserver.org/what-we-do/network-reporting/

## I. News (discovery only)

- BleepingComputer: https://www.bleepingcomputer.com/
- Hacker News: https://thehackernews.com/
- SecurityWeek: https://www.securityweek.com/
- The Record: https://therecord.media/
- Help Net Security: https://www.helpnetsecurity.com/

## Maintenance (per setup)

Validate each URL, discover feeds via official docs, record auth/subscription needs, note freshness, flag redirects/retired/broken, add missing vendor sources for monitored products.
