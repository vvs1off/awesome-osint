<div align="center">

# Awesome OSINT

**A curated list of Open Source Intelligence tools, methods and learning material<br>for researchers, journalists, security assessors and investigators.**

[![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/license-CC0--1.0-111111?style=flat-square)](LICENSE)
[![Link check](https://github.com/vvs1off/awesome-osint/actions/workflows/link-check.yml/badge.svg)](https://github.com/vvs1off/awesome-osint/actions/workflows/link-check.yml)

</div>

> [!CAUTION]
> **Ethics & legal notice.** This list is for **authorized security assessments, journalism, academic research and lawful investigations only**.
> OSINT must respect applicable law (for example the [GDPR](https://gdpr-info.eu/) in the EU), each platform's terms of service, and the people behind the data.
> Do not use these resources to stalk, harass, dox, intimidate or profile private individuals, and never buy or trade leaked personal data.
> "Publicly available" is not the same as "fair to collect": minimise what you gather, document your lawful basis, and stop when you lack one.
> Inclusion here is not an endorsement; you are responsible for how you use any tool.

## Contents

- [Ethics & Legal](#ethics--legal)
- [Frameworks & Methodology](#frameworks--methodology)
- [Search Engines & Dorking](#search-engines--dorking)
- [Web Archiving & Evidence Capture](#web-archiving--evidence-capture)
- [Username & Account Search](#username--account-search)
- [Email & Breach Awareness](#email--breach-awareness)
- [Domain, IP & Infrastructure](#domain-ip--infrastructure)
- [Recon Frameworks](#recon-frameworks)
- [Social Media Analysis](#social-media-analysis)
- [Image Analysis & Geolocation](#image-analysis--geolocation)
- [Maps & Geospatial](#maps--geospatial)
- [Transport Tracking](#transport-tracking)
- [Companies & Public Records](#companies--public-records)
- [Documents & Metadata](#documents--metadata)
- [Threat Intelligence](#threat-intelligence)
- [Learning Resources](#learning-resources)
- [Books](#books)
- [Blogs & Research](#blogs--research)
- [Communities](#communities)
- [Related Lists](#related-lists)
- [Contributing](#contributing)
- [License](#license)

---

## Ethics & Legal

- [Berkeley Protocol on Digital Open Source Investigations](https://www.ohchr.org/en/publications/policy-and-methodological-publications/berkeley-protocol-digital-open-source) - UN OHCHR standard for collecting, preserving and verifying open-source evidence.
- [GDPR (consolidated text)](https://gdpr-info.eu/) - Searchable text of the EU General Data Protection Regulation.
- [ICO guide to UK GDPR](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/) - Regulator guidance on lawful basis, legitimate interests and data minimisation.

## Frameworks & Methodology

- [OSINT Framework](https://osintframework.com/) - Interactive tree of OSINT resources grouped by data type.
- [Bellingcat Online Investigations Toolkit](https://bellingcat.gitbook.io/toolkit) - Community-maintained catalogue of tools with usage notes and caveats.
- [MITRE ATT&CK: Reconnaissance (TA0043)](https://attack.mitre.org/tactics/TA0043/) - Adversary recon techniques; useful for scoping what defenders expose.
- [OWASP WSTG: Information Gathering](https://wstg.owasp.org/stable/4-Web_Application_Security_Testing/01-Information_Gathering/) - Recon phase of the OWASP Web Security Testing Guide.
- [Verification Handbook](https://datajournalism.com/read/handbook/verification-3) - Free handbook on verifying digital content and investigating disinformation.

## Search Engines & Dorking

- [Google Search Operators](https://developers.google.com/search/docs/monitor-debug/search-operators) - Official reference for `site:`, `filetype:` and related operators.
- [Google Hacking Database](https://www.exploit-db.com/google-hacking-database) - Exploit-DB's catalogue of dorks that surface exposed files and misconfigurations.
- [DuckDuckGo Search Syntax](https://duckduckgo.com/duckduckgo-help-pages/results/syntax) - Operators supported by DuckDuckGo.
- [Yandex](https://yandex.com/) - Search engine with strong coverage of Russian-language sources.
- [Baidu](https://www.baidu.com/) - Leading search engine for Chinese-language sources.
- [grep.app](https://grep.app/) - Fast regex search across public Git repositories.
- [PublicWWW](https://publicwww.com/) - Search web page source code for snippets, tracking IDs and libraries.
- [Common Crawl](https://commoncrawl.org/) - Open, petabyte-scale web crawl archive for large-scale research.

## Web Archiving & Evidence Capture

- [Wayback Machine](https://web.archive.org/) - Internet Archive's historical snapshots of web pages, with on-demand saving.
- [ArchiveBox](https://github.com/ArchiveBox/ArchiveBox) - Self-hosted archiver that saves pages as HTML, PDF, screenshot and WARC.
- [Auto Archiver](https://github.com/bellingcat/auto-archiver) - Bellingcat tool to archive social media posts and media at scale.
- [ArchiveWeb.page](https://webrecorder.net/archivewebpage/) - Webrecorder browser extension for high-fidelity WARC capture.
- [Hunchly](https://hunch.ly/) - Commercial browser extension that logs and hashes every page visited during an investigation.

## Username & Account Search

> Use only within an authorized scope (e.g. assessing an organisation's own exposure, or a consenting subject). Matching usernames are leads, not proof of identity.

- [Sherlock](https://github.com/sherlock-project/sherlock) - CLI that checks a username across hundreds of sites.
- [Maigret](https://github.com/soxoj/maigret) - Sherlock fork that also parses public profile pages and builds reports.
- [WhatsMyName](https://github.com/WebBreacher/WhatsMyName) - Community-maintained dataset of username-check rules, with a [web front end](https://whatsmyname.app/).

## Email & Breach Awareness

> Defensive framing: check your own or your organisation's exposure, notify, and rotate credentials. Do not seek out or purchase breach dumps.

- [Have I Been Pwned](https://haveibeenpwned.com/) - Check whether an email or domain appears in known breaches; supports domain-wide monitoring.
- [Pwned Passwords](https://haveibeenpwned.com/Passwords) - k-anonymity API to test passwords against breach corpora without revealing them.
- [Mozilla Monitor](https://monitor.mozilla.org/) - Breach alerts for your own email addresses.
- [Google Admin Toolbox Messageheader](https://toolbox.googleapps.com/apps/messageheader/) - Parse email headers to trace delivery path and authentication results.
- [MXToolbox](https://mxtoolbox.com/) - MX, SPF, DMARC and blacklist checks for mail infrastructure.
- [Hunter](https://hunter.io/) - Find the email address format used by an organisation.

## Domain, IP & Infrastructure

- [Shodan](https://www.shodan.io/) - Search engine for internet-connected devices and exposed services.
- [Censys](https://censys.com/) - Internet-wide scan data for hosts and certificates.
- [Netlas](https://netlas.io/) - Search engine for hosts, domains, certificates and WHOIS records.
- [crt.sh](https://crt.sh/) - Certificate Transparency log search; great for subdomain discovery.
- [ICANN Lookup](https://lookup.icann.org/) - Official RDAP/WHOIS lookup for domain registration data.
- [SecurityTrails](https://securitytrails.com/) - Historical DNS, WHOIS and subdomain data.
- [DNSDumpster](https://dnsdumpster.com/) - Free DNS recon and host mapping.
- [ViewDNS.info](https://viewdns.info/) - Reverse IP, reverse WHOIS and other DNS utilities.
- [urlscan.io](https://urlscan.io/) - Sandbox that scans and records what a URL loads and contacts.
- [Hurricane Electric BGP Toolkit](https://bgp.he.net/) - ASN, prefix and peering information.
- [bgp.tools](https://bgp.tools/) - Modern BGP and ASN explorer.
- [RIPEstat](https://stat.ripe.net/) - RIPE NCC data on IP space, routing and registration.
- [BuiltWith](https://builtwith.com/) - Technology profiling of websites.
- [Wappalyzer](https://www.wappalyzer.com/) - Browser extension that identifies site technologies.
- [dnstwist](https://github.com/elceef/dnstwist) - Find look-alike domains for phishing and brand-abuse monitoring.

## Recon Frameworks

- [SpiderFoot](https://github.com/smicallef/spiderfoot) - Automated OSINT collection with 200+ modules and a web UI.
- [theHarvester](https://github.com/laramies/theHarvester) - Gathers emails, subdomains, hosts and names from public sources.
- [Recon-ng](https://github.com/lanmaster53/recon-ng) - Modular, Metasploit-style web reconnaissance framework.
- [OWASP Amass](https://github.com/owasp-amass/amass) - In-depth attack surface mapping and subdomain enumeration.
- [Subfinder](https://github.com/projectdiscovery/subfinder) - Fast passive subdomain discovery.

## Social Media Analysis

> Prefer official research APIs and platform search. Respect rate limits and terms of service, and avoid collecting data on private individuals beyond your stated purpose.

- [InVID-WeVerify Plugin](https://www.invid-project.eu/tools-and-services/invid-verification-plugin/) - Browser plugin for video and image verification (keyframes, metadata, reverse search).
- [4CAT](https://github.com/digitalmethodsinitiative/4cat) - Research tool for capturing and analysing social media datasets.
- [Meta Content Library](https://transparency.meta.com/researchtools/meta-content-library) - Official research access to public Facebook and Instagram content.
- [TikTok Research API](https://developers.tiktok.com/products/research-api/) - Official API for qualified academic researchers.
- [YouTube Data Tools](https://ytdt.digitalmethods.net/) - Extract channel, video and comment networks via the YouTube API.
- [TGStat](https://tgstat.com/) - Analytics and search for public Telegram channels.

## Image Analysis & Geolocation

- [Google Lens](https://lens.google/) - Reverse image and object search.
- [TinEye](https://tineye.com/) - Reverse image search with first-seen sorting.
- [Yandex Images](https://yandex.com/images/) - Reverse image search strong on landmarks and buildings.
- [ExifTool](https://exiftool.org/) - The reference tool for reading and writing file metadata.
- [FotoForensics](https://fotoforensics.com/) - Error level analysis and metadata for spotting manipulation.
- [Forensically](https://29a.ch/photo-forensics/) - In-browser clone detection, ELA and noise analysis.
- [SunCalc](https://www.suncalc.org/) - Sun position and shadow direction for any place and time; used for chronolocation.
- [PeakVisor](https://peakvisor.com/) - 3D mountain panoramas for matching ridgelines.
- [Bellingcat OpenStreetMap Search](https://osm-search.bellingcat.com/) - Find locations by combinations of nearby map features.

## Maps & Geospatial

- [Google Earth](https://earth.google.com/web/) - Satellite imagery, 3D terrain and historical imagery in the browser.
- [OpenStreetMap](https://www.openstreetmap.org/) - Collaborative open map data.
- [Overpass Turbo](https://overpass-turbo.eu/) - Query OpenStreetMap data for specific features.
- [Copernicus Browser](https://browser.dataspace.copernicus.eu/) - Free Sentinel satellite imagery with time series.
- [NASA Worldview](https://worldview.earthdata.nasa.gov/) - Near-real-time global satellite imagery.
- [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/map/) - Active fire and thermal anomaly data.
- [USGS EarthExplorer](https://earthexplorer.usgs.gov/) - Landsat and other historical imagery archives.
- [Zoom Earth](https://zoom.earth/) - Live satellite weather and imagery map.
- [Mapillary](https://www.mapillary.com/) - Crowdsourced street-level imagery.
- [KartaView](https://kartaview.org/) - Open street-level imagery platform.

## Transport Tracking

- [ADS-B Exchange](https://globe.adsbexchange.com/) - Unfiltered community flight tracking.
- [Flightradar24](https://www.flightradar24.com/) - Live and historical flight tracking.
- [OpenSky Network](https://opensky-network.org/) - Open ADS-B research data.
- [MarineTraffic](https://www.marinetraffic.com/) - AIS vessel tracking.
- [Global Fishing Watch](https://globalfishingwatch.org/platform/map) - Vessel activity and fishing effort map.

## Companies & Public Records

- [OpenCorporates](https://opencorporates.com/) - Largest open database of company registrations.
- [SEC EDGAR Full-Text Search](https://www.sec.gov/edgar/search/) - Search US public company filings.
- [UK Companies House](https://find-and-update.company-information.service.gov.uk/) - UK company records, officers and filings.
- [GLEIF LEI Search](https://search.gleif.org/) - Global Legal Entity Identifier registry and ownership links.
- [OpenSanctions](https://www.opensanctions.org/) - Consolidated sanctions lists and politically exposed persons data.
- [ICIJ Offshore Leaks Database](https://offshoreleaks.icij.org/) - Offshore entities published from ICIJ investigations.
- [OCCRP Aleph](https://aleph.occrp.org/) - Investigative data platform with public records and leaks for journalists.
- [Company Social Profile Finder](https://apify.com/publicrecords/company-social-profile-finder) - Company domain or name to its LinkedIn, X, YouTube, Instagram and Facebook links, with confidence scores (Apify Actor, API + MCP, free tier).
- [USAspending Awards Scraper](https://apify.com/publicrecords/usaspending-awards-scraper) - US federal contract and grant awards by agency, recipient, NAICS and period (Apify Actor, API + MCP, free tier).
- [Grants.gov Scraper](https://apify.com/publicrecords/grants-gov-scraper) - Open US federal grants: agency, deadline, eligibility and source link (Apify Actor, API + MCP, free tier).
- [Federal Contracts Feed (SAM.gov + Grants.gov)](https://apify.com/publicrecords/govcon-opportunity-feed) - New US federal contract and grant notices from SAM.gov and Grants.gov in one feed (Apify Actor, API + MCP, free tier).
- [City Council Meetings Scraper (Legistar)](https://apify.com/publicrecords/legistar-meetings-scraper) - City council meetings, agenda items and documents for any Legistar city (Apify Actor, API + MCP, free tier).
- [EU TED Tenders Scraper](https://apify.com/publicrecords/eu-ted-notices-scraper) - EU procurement notices from TED: buyer, CPV, value, deadline, link (Apify Actor, API + MCP, free tier).
- [UK Tenders Scraper](https://apify.com/publicrecords/uk-find-a-tender-scraper) - UK government tenders from Find a Tender and Contracts Finder: buyer, value, deadline (Apify Actor, API + MCP, free tier).

## Documents & Metadata

- [FOCA](https://github.com/ElevenPaths/FOCA) - Extract metadata and hidden information from documents found on a domain.
- [Metagoofil](https://github.com/opsdisk/metagoofil) - Find public documents for a domain and pull their metadata.
- [Apache Tika](https://tika.apache.org/) - Extract text and metadata from over a thousand file types.
- [DocumentCloud](https://www.documentcloud.org/) - Analyse, annotate and publish primary source documents.
- [mat2](https://0xacab.org/jvoisin/mat2) - Remove metadata from your own files before publishing (defensive).

## Threat Intelligence

- [VirusTotal](https://www.virustotal.com/) - Multi-engine file, URL, domain and IP reputation.
- [URLhaus](https://urlhaus.abuse.ch/) - abuse.ch feed of malware distribution URLs.
- [MalwareBazaar](https://bazaar.abuse.ch/) - abuse.ch malware sample sharing.
- [ThreatFox](https://threatfox.abuse.ch/) - abuse.ch IOC sharing platform.
- [AlienVault OTX](https://otx.alienvault.com/) - Community threat intelligence pulses and IOCs.
- [AbuseIPDB](https://www.abuseipdb.com/) - Crowdsourced IP abuse reports.
- [GreyNoise](https://viz.greynoise.io/) - Separates internet background noise from targeted activity.
- [Pulsedive](https://pulsedive.com/) - Free threat intelligence enrichment.
- [PhishTank](https://phishtank.org/) - Community-verified phishing URLs.
- [Hybrid Analysis](https://hybrid-analysis.com/) - Free malware sandbox reports.
- [CISA KEV Catalog](https://www.cisa.gov/known-exploited-vulnerabilities-catalog) - Vulnerabilities known to be exploited in the wild.
- [MISP](https://www.misp-project.org/) - Open-source threat intelligence sharing platform.
- [OpenCTI](https://github.com/OpenCTI-Platform/opencti) - Open-source platform for managing cyber threat intelligence.

## Learning Resources

- [Trace Labs](https://www.tracelabs.org/) - OSINT search party CTFs that help find missing persons with law enforcement.
- [Bellingcat Guides](https://www.bellingcat.com/category/resources/how-tos/) - Step-by-step investigation tutorials.
- [GIJN Resource Center](https://gijn.org/resource-center/) - Global Investigative Journalism Network guides and tipsheets.
- [SANS SEC497](https://www.sans.org/cyber-security-courses/practical-open-source-intelligence) - Practical OSINT course.
- [Week in OSINT](https://sector035.nl/) - Weekly roundup of new tools and techniques.
- [OSINT Curious](https://www.osintcurio.us/) - Community project with articles, webcasts and live streams.

## Books

- *Open Source Intelligence Techniques* - Michael Bazzell. [Publisher page](https://inteltechniques.com/book1.html). The long-running practitioner's manual.
- *Extreme Privacy* - Michael Bazzell. [Publisher page](https://inteltechniques.com/book7.html). The defensive counterpart: reducing your own exposure.
- *Deep Dive: Exploring the Real-world Value of Open Source Intelligence* - Rae L. Baker. [Wiley](https://www.wiley.com/en-us/Deep+Dive%3A+Exploring+the+Real+world+Value+of+Open+Source+Intelligence-p-9781119933243). OSINT across disciplines.
- *We Are Bellingcat* - Eliot Higgins. [Bloomsbury](https://www.bloomsbury.com/uk/we-are-bellingcat-9781526615725/). The story and methods of open-source investigation.
- *Digital Witness* - Sam Dubberley, Alexa Koenig, Daragh Murray (eds.). [Oxford University Press](https://global.oup.com/academic/product/digital-witness-9780198836070). Open-source information for human rights work.

## Blogs & Research

- [Bellingcat](https://www.bellingcat.com/) - Independent investigative collective pioneering open-source methods.
- [DFRLab](https://dfrlab.org/) - Atlantic Council lab on disinformation and digital forensics.
- [The Citizen Lab](https://citizenlab.ca/) - Research on spyware, censorship and digital threats to civil society.
- [Forensic Architecture](https://forensic-architecture.org/) - Spatial and architectural analysis of human rights violations.
- [C4ADS](https://c4ads.org/) - Data-driven analysis of illicit networks and conflict.
- [The DFIR Report](https://thedfirreport.com/) - Detailed real-world intrusion reports with IOCs.
- [NixIntel](https://nixintel.info/) - Practical OSINT and geolocation write-ups.

## Communities

- [r/OSINT](https://www.reddit.com/r/OSINT/) - Reddit community for tools, techniques and questions.
- [OSINT Foundation](https://www.osintfoundation.com/) - Professional association for OSINT practitioners.
- [GIJN](https://gijn.org/) - Global network of investigative journalism organisations.

## Related Lists

- [jivoi/awesome-osint](https://github.com/jivoi/awesome-osint) - Large, long-standing OSINT link collection.
- [sindresorhus/awesome](https://github.com/sindresorhus/awesome) - The original list of awesome lists.

## Contributing

Contributions are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) first: every entry must be legitimate, publicly available and consistent with the ethics notice above.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related rights to this work. See [LICENSE](LICENSE).
