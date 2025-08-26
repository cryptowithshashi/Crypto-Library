---
title: "Anti-Money Laundering (AML) & Compliance"
slug: "aml-compliance"
filename: "A-AML-Compliance.md"
tags: ["aml","compliance","kyc","kyb","sanctions","regulation","on-chain","off-chain"]
difficulty: "Intermediate"
jurisdictions: ["global"]
last_updated: "2025-08-26"
maintainer: "handle@example.org"
license: "CC-BY-4.0"
---

# Anti-Money Laundering (AML) & Compliance

Comprehensive resource covering AML/CFT compliance for cryptocurrency and traditional finance, including regulatory guidance, implementation tools, and operational playbooks.

# Reading Pathways

## Quick Start

* [FATF Virtual Assets Guidance](https://www.fatf-gafi.org/en/publications/Fatfrecommendations/Guidance-rba-virtual-assets-2021.html) : Core regulatory framework.
* [FinCEN: Application of FinCEN's Regulations to Persons Administering, Exchanging, or Using Virtual Currencies](https://www.fincen.gov/sites/default/files/shared/FIN-2013-G001.pdf) : Core US guidance on how BSA/AML rules apply to virtual currency businesses.
* [AUSTRAC: A guide to preparing and implementing an AML/CTF program for your digital currency exchange business](https://www.austrac.gov.au/business/how-comply-guidance-and-resources/guidance-resources/guide-preparing-and-implementing-amlctf-program-your-digital-currency-exchange-business) : Practical checklist + sample controls for crypto exchanges.

## Implementation

* [Elliptic AML API docs](https://developers.elliptic.co/docs/getting-started) : API quickstart for batch/real-time KYT screening and developer examples.
* [Chainalysis KYT product page & docs](https://www.chainalysis.com/product/kyt/) : KYT integration patterns, risk scoring and workflows for exchanges.
* [Ethereum ETL / blockchain-etl (GitHub)](https://github.com/blockchain-etl/ethereum-etl) : ETL tooling to export blockchain data to CSV/BigQuery for monitoring/backtests.
* [FATF Travel Rule Implementation](https://sumsub.com/blog/what-is-the-fatf-travel-rule/) : Technical requirements and thresholds.
* [Sample SAR Filing Workflow](https://www.fincen.gov/sites/default/files/shared/report_reference.pdf) : Operational procedures.
* [BSA/AML Policy Templates](https://dilendorf.com/resources/bsa-aml-policies-for-cryptocurrency-exchanges-and-defi-applications-in-a-nutshell.html) : Policy frameworks.

## Research & Legal

* [FATF: Guidance for a Risk-Based Approach to Virtual Assets and VASPs](https://www.fatf-gafi.org/publications/fatfrecommendations/documents/guidance-rba-virtual-assets.html) : FATF’s baseline expectations for VASPs (Travel Rule, CDD, risk-based approach).
* [Directive (EU) 2018/843 (AMLD5)](https://eur-lex.europa.eu/legal-content/EN/NIM/?uri=OJ%3AJOL_2018_156_R_0003) : EU AML changes relevant to crypto and transparency measures.
* [“Anti-money laundering in Bitcoin” (Elliptic dataset & paper)](https://arxiv.org/abs/1908.02591) : Public labeled dataset useful for detection model development and backtesting.
* [EU 5th & 6th AML Directives](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32018L0843) : European requirements.
* [Academic Papers on Cryptocurrency AML](https://arxiv.org/list/cs.CY/recent) : Research developments.
* [UNODC Money Laundering Typologies](https://www.unodc.org/unodc/en/money-laundering/overview.html) : Global patterns analysis.

## 1. Official Guidance & Regulator References

## International Standards

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [FATF Recommendations](https://www.fatf-gafi.org/en/publications/Fatfrecommendations/Fatf-recommendations.html) | FATF-GAFI | (Official guidance; 2023) Core 40 recommendations for AML/CFT framework globally. [note: PDF download] |
| [Virtual Assets: Updated Guidance 2021](https://www.fatf-gafi.org/en/publications/Fatfrecommendations/Guidance-rba-virtual-assets-2021.html) | FATF-GAFI | (Official guidance; 2021) Risk-based approach for VAs and VASPs with travel rule clarifications. |
| [Targeted Update on Virtual Assets 2025](https://www.fatf-gafi.org/en/publications/Fatfrecommendations/targeted-update-virtual-assets-vasps-2025.html) | FATF-GAFI | (Assessment report; 2025) Sixth update on global VA/VASP implementation compliance status. |

---

## United States

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [FinCEN Virtual Currency Guidance](https://www.fincen.gov/resources/statutes-regulations/guidance/application-fincens-regulations-persons-administering) | US Treasury | (Official guidance; 2013) MSB registration requirements for virtual currency businesses. |
| [FinCEN CVC Guidance 2019](https://www.fincen.gov/sites/default/files/2019-05/FinCEN%20Guidance%20CVC%20FINAL%20508.pdf) | US Treasury | (Official guidance; 2019) Comprehensive BSA application to cryptocurrency business models. [note: PDF] |
| [BSA Requirements](https://www.fdic.gov/resources/supervision-and-examinations/examination-policies-manual/section8-1.pdf) | FinCEN | (Statute; 1970) Bank Secy Act foundational requirements and reporting. |

## 2.  Laws & Requirements by Region

### Global/FATF

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [FATF Standards](https://www.fatf-gafi.org/en/publications/Fatfrecommendations/Fatf-recommendations.html) | FATF-GAFI | (International standard; 2023) 40 Recommendations plus 9 Special Recommendations on terrorist financing.|

>**Key requirements:** $1,000/€1,000 travel rule threshold, VASP licensing, beneficial ownership registries. 


### United States

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Bank Secrecy Act](https://www.fdic.gov/resources/supervision-and-examinations/examination-policies-manual/section8-1.pdf) | FinCEN | (Federal statute; 1970) Core AML law requiring MSB registration and SAR filing. |
| [USA PATRIOT Act](https://www.congress.gov/bill/107th-congress/house-bill/3162) | Congress | (Federal statute; 2001) Enhanced due diligence and customer identification requirements.|

>**Key requirements:** $10,000 CTR threshold, $3,000 travel rule (proposed $250), MSB registration for VASPs.

### European Union

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [5th Anti-Money Laundering Directive](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32018L0843) | EU | (EU Directive; 2018) Extends AML to crypto exchanges and custodial wallet providers. |
| [6th Anti-Money Laundering Directive](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32018L1673) | EU | (EU Directive; 2018) Harmonizes money laundering criminal offenses across member states.|

>**Key requirements:** €1,000 travel rule threshold, VASP registration, UBO registries, enhanced CDD. 

### United Kingdom

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Money Laundering Regulations 2017](https://www.legislation.gov.uk/uksi/2017/692/contents/made) | HMRC | (UK Statute; 2017) Implements EU directives with crypto exchange supervision by FCA. |
| [FCA Cryptoasset Guidance](https://www.fca.org.uk/publication/guidance/fg19-03.pdf) | UK FCA | (Official guidance; 2019) Registration and compliance requirements for crypto businesses.|

>**Key requirements:** £1,000 travel rule threshold, FCA registration required, enhanced CDD for high-risk customers. 

### India

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Prevention of Money Laundering Act](https://fiuindia.gov.in/files/AML_Legislation/pmla_2002.html) | India | (Indian statute; 2002) PMLA requirements with FIU-IND reporting obligations. |
| [RBI Virtual Currency Guidelines](https://www.rbi.org.in/Scripts/NotificationUser.aspx?Id=12103) | Reserve Bank | (Official guidance; 2018) Banking restrictions and regulatory approach to virtual currencies.|

>**Key requirements:** ₹50,000 threshold for enhanced CDD, suspicious transaction reporting to FIU-IND. 

### Singapore

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Payment Services Act](https://www.mas.gov.sg/regulation/acts/payment-services-act) | MAS | (Singapore statute; 2019) Licensing framework for digital payment token services. |
| [MAS AML/CFT Guidelines](https://www.mas.gov.sg/regulation/guidelines/guidelines-to-notice-psn02-on-aml-and-cft---dpt) | Singapore MAS | (Official guidance; 2020) AML/CFT requirements for payment service providers.|

>**Key requirements:** S$1,000 travel rule threshold, MAS licensing for DPT services, risk-based CDD. 

### Hong Kong

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Anti-Money Laundering Ordinance](https://www.elegislation.gov.hk/hk/cap615) | Hong Kong | (HK statute; 2012) AMLO requirements for financial institutions and designated non-financial businesses. |
| [SFC Virtual Asset Guidelines](https://www.sfc.hk/en/regulatory-functions/intermediaries/supervision/virtual-asset-trading-platforms) | Hong Kong SFC | (Official guidance; 2023) Licensing and conduct requirements for VA trading platforms.|

>**Key requirements:** HK$8,000 travel rule threshold, SFC licensing for VA platforms, professional investor restrictions. 

### Australia

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Anti-Money Laundering Act 2006](https://www.austrac.gov.au/business/how-comply-guidance-and-resources/guidance-resources/anti-money-laundering-and-counter-terrorism-financing-amlctf-act) | AUSTRAC | (Australian statute; 2006) AML/CTF Act requirements for reporting entities including digital currency exchanges. |
| [AUSTRAC Digital Currency Exchange Guidelines](https://www.austrac.gov.au/business/how-comply-guidance-and-resources/guidance-resources/digital-currency-exchange-dce-registration-and-reporting) | AUSTRAC | (Official guidance; 2018) Registration and reporting obligations for DCEs.|

>**Key requirements:** A$10,000 threshold transactions, DCE registration with AUSTRAC, suspicious matter reporting. 

## 3. KYC / KYB Basics (Identity Verification)

### KYC Fundamentals

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Customer Due Diligence Rule](https://www.fincen.gov/resources/statutes-and-regulations/cdd-final-rule) | FinCEN | (Federal regulation; 2016) CDD requirements including beneficial ownership identification procedures. |
| [KYC Standards Guide](https://www.fatf-gafi.org/en/publications/Fatfrecommendations/Guidance-rba-virtual-assets-2021.html) | FATF | (Official guidance; 2021) Customer identification and verification standards for VASPs. |
| [Jumio Identity Verification Guide](https://www.jumio.com/products/authentication/) | Jumio | (Industry guide; 2024) Document verification, biometric matching, and liveness detection methods. |

---

### KYB & Beneficial Ownership

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Beneficial Ownership Information](https://www.fincen.gov/beneficial-ownership-information-reporting-requirements) | FinCEN | (Official guidance; 2024) Corporate Transparency Act reporting requirements for beneficial ownership. [note: Updated March 2025] |
| [UBO Register Guidelines](https://ec.europa.eu/info/business-economy-euro/company-reporting-and-auditing/company-information/beneficial-ownership-registers_en) | EU | (EU guidance; 2019) Ultimate beneficial ownership registry access and verification procedures. |
| [Onfido KYB Solutions](https://onfido.com/solutions/kyb/) | Onfido | (Vendor docs; 2024) Business verification API with UBO screening and sanctions checking. [pricing: contact sales] |

---

### Identity Verification Providers

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Persona Identity Platform](https://withpersona.com/docs) | Persona | (API docs; 2024) Identity verification with document capture, biometric matching, real-time decision engine. [pricing: per verification] |
| [Veriff Identity Verification](https://www.veriff.com/developers) | Veriff | (API docs; 2024) Document verification supporting 10,000+ documents from 230+ countries. [pricing: tiered] |
| [Entrust (Onfido) Identity Verification API docs](https://documentation.onfido.com/api/latest/) | Entrust / Onfido | (Doc; 2024) API quickstart for document & biometric identity verification. [note: API-key required] |
| [Trulioo GlobalGateway Developer Portal](https://developer.trulioo.com/reference/welcome) | Trulioo | (Doc; ongoing) Global identity & business verification flows; integration recipes. [note: API-key required] |


## 4. Transaction Monitoring & Detection (TM)

### Blockchain Analytics & Red Flags

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Chainalysis KYT (Know Your Transaction)](https://www.chainalysis.com/product/kyt/) | Chainalysis | (Doc; 2024) KYT product overview, risk scoring, and integration patterns. [note: demo / sales contact] |
| [Elliptic AML API docs (developers)](https://developers.elliptic.co/docs/getting-started) | Elliptic | (Doc; 2024) Batch and programmatic transaction/wallet screening examples. [note: API-key required] |
| [Indicators of suspicious activity for digital currency sector](https://www.austrac.gov.au/business/how-comply-guidance-and-resources/guidance-resources/indicators-suspicious-activity-digital-currency-cryptocurrency-sector) | AUSTRAC | (Guidance; 2025) Concrete red flags to feed into TM rules. [note: free] |

---

### Monitoring Frameworks

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Transaction Monitoring Best Practices](https://www.acams.org/transaction-monitoring/) | ACAMS | (Industry guide; 2024) Rule calibration, alert management, and false positive reduction strategies. |
| [SAR Narratives Guide](https://www.acams.org/sar-narratives/) | ACAMS | (Training resource; 2024) Sample SAR narratives and suspicious activity identification techniques. |
| [SWIFT KYC Registry](https://www.swift.com/our-solutions/compliance-and-shared-services/financial-crime-compliance/kyc-registry) | SWIFT | (Industry service; 2024) Centralized KYC data sharing for correspondent banking relationships. |

---

### Rule Types & Pattern Detection

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [FinCEN SAR Stats & Trends](https://www.fincen.gov/reports/sar-stats) | US Treasury | (Statistical report; 2024) Annual suspicious activity reporting statistics and emerging typologies. |
| [UNODC Money Laundering Methods](https://www.unodc.org/unodc/en/money-laundering/laundry-methods.html) | UN | (Educational resource; 2024) Money laundering techniques including structuring, layering, and integration methods. |
| [Actimize Transaction Monitoring](https://www.niceactimize.com/financial-crime/transaction-monitoring/) | NICE | (Vendor solution; 2024) Real-time monitoring with machine learning-based rule optimization. [pricing: enterprise] |

---

### Stream Processing & Analytics

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Apache Kafka for Financial Services](https://www.confluent.io/use-case/financial-services/) | Confluent | (Technical guide; 2024) Real-time data streaming architecture for transaction monitoring pipelines. |
| [Elasticsearch Security Analytics](https://www.elastic.co/security) | Elastic | (Product docs; 2024) Search and analytics platform for financial crime detection use cases. [pricing: subscription tiers] |

## 5. Clustering & Analytics Heuristics (On-Chain Analytics)


### Address Clustering Techniques

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Address Clustering in Bitcoin](https://arxiv.org/abs/1502.01657) | Academic Research | (Research paper; 2015) Multi-input and change address heuristics for Bitcoin transaction graph analysis. [note: foundational paper] |
| [Chainalysis Reactor Methodology](https://blog.chainalysis.com/reports/cryptocurrency-clustering/) | Chainalysis | (Methodology whitepaper; 2023) Proprietary clustering algorithms and attribution confidence scores for cryptocurrency investigations. |
| [Elliptic Investigation Tools](https://www.elliptic.co/investigation) | Elliptic | (Product documentation; 2024) Graph analysis tools with clustering heuristics and risk scoring methodologies. [pricing: subscription] |

---

### Evaluation & Limitations

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Clustering Precision Analysis](https://dci.mit.edu/research) | MIT | (Research; 2022) Analysis of clustering heuristic accuracy rates and false positive risks in Bitcoin. [note: limitations emphasized] |
| [Privacy Coin Analysis](https://www.rand.org/pubs/research_reports/RRA465-1.html) | RAND Corporation | (Policy research; 2020) Technical analysis of Monero, Zcash traceability with regulatory implications. [note: ethical considerations] |

---

### Public Datasets & Benchmarks

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Bitcoin Address Dataset](https://www.bitcoinabuse.com/api-docs) | BitcoinAbuse | (Public dataset; 2024) Crowdsourced database of cryptocurrency addresses used in crimes. [API: rate limited] |
| [Crystal Blockchain Analytics](https://crystalblockchain.com/) | Bitfury | (Commercial platform; 2024) Investigation tools with graph visualization and risk assessment scoring. [pricing: enterprise] |
| [A Fistful of Bitcoins: Characterizing Payments Among Men with No Names](https://cseweb.ucsd.edu/~smeiklejohn/files/imc13.pdf) | Meiklejohn et al. | (Paper; 2013) Original heuristics and clustering for Bitcoin address attribution. [note: PDF] |
| [Anti-money laundering in Bitcoin](https://arxiv.org/abs/1908.02591) | Elliptic / Academic | (Paper; 2019) Graph ML approaches and labeled transaction dataset. [note: dataset on Kaggle] |
| [GraphSense (open-source analytics platform)](https://graphsense.org/) | GraphSense | (Tool/Repo; active) Open analytics platform for clustering, entity resolution. [note: open-source] |


## 6. Sanctions Screening & Watchlists

### Official Sanctions Lists

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [OFAC SDN List](https://www.treasury.gov/ofac/downloads/sdnlist.pdf) | US Treasury | (Official list; 2025) Specially Designated Nationals list; downloadable CSV & API; daily updates. [note: real-time API available] |
| [EU Consolidated List](https://www.consilium.europa.eu/en/policies/sanctions/restrictive-measures-against-persons-entities/) | European External Action Service | (Official list; 2025) EU restrictive measures database with person and entity listings; weekly updates. |
| [UN Security Council Sanctions](https://www.un.org/securitycouncil/sanctions/information) | UN | (Official list; 2025) UN Security Council sanctions committee consolidated list; monthly updates. |
| [UK HM Treasury Sanctions](https://www.gov.uk/government/publications/financial-sanctions-consolidated-list-of-targets) | UK HMT | (Official list; 2025) UK financial sanctions targets list; Excel/CSV format; weekly updates. |

### PEP & Adverse Media Screening

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [World-Check Risk Intelligence](https://www.refinitiv.com/en/products/world-check-risk-intelligence) | Refinitiv | (Commercial service; 2024) PEP and sanctions screening database with adverse media monitoring. [pricing: subscription] |
| [Dow Jones Risk & Compliance](https://professional.dowjones.com/risk/) | Dow Jones | (Commercial service; 2024) PEP database and adverse media screening with real-time alerts. [pricing: per search/subscription] |
| [LexisNexis PoliticallyExposed](https://risk.lexisnexis.com/products/politically-exposed-persons) | LexisNexis | (Commercial service; 2024) PEP identification and monitoring with relationship mapping capabilities. [pricing: enterprise] |

---

### Crypto-Specific Screening

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Chainalysis Sanctions Screening](https://www.chainalysis.com/free-cryptocurrency-sanctions-screening-tools/) | Chainalysis | (Free tool; 2024) Free sanctions screening for cryptocurrency addresses with OFAC compliance. [API: freemium model] |
| [Elliptic Navigator](https://www.elliptic.co/navigator) | Elliptic | (Commercial tool; 2024) Real-time crypto sanctions screening with wallet and exchange integration. [pricing: per API call] |

## 7. Compliance Providers & Vendor Comparisons

### KYC/KYB Providers

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Jumio Identity Verification](https://www.jumio.com/platform/) | Jumio | (Platform docs; 2024) Document verification, biometric authentication, fraud prevention; supports 5,000+ ID types.<br>[pricing: per verification; API: REST; chains: BTC/ETH integrations] |
| [Onfido Identity Platform](https://documentation.onfido.com/) | Onfido | (API docs; 2024) Identity verification with AI-powered document authentication and facial biometrics.<br>[pricing: tiered; API: REST/webhooks; integration: major exchanges] |
| [Persona Identity Infrastructure](https://docs.withpersona.com/) | Persona | (Developer docs; 2024) Configurable identity verification flows with risk-based decisioning.<br>[pricing: per check; API: GraphQL; sample: risk_score, verification_status] |

---

### Transaction Monitoring (KYT)

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Chainalysis KYT](https://www.chainalysis.com/products/kyt/) | Chainalysis | (Product page; 2024) Real-time crypto transaction monitoring with risk scoring and compliance reporting.<br>[chains: 20+ supported; pricing: enterprise; API: REST; sample: {risk_score: 0.8, exposure: "high", labels: ["mixer"]}] |
| [Elliptic Lens](https://www.elliptic.co/products/lens) | Elliptic | (Product page; 2024) Cryptocurrency compliance and investigation platform with transaction tracing.<br>[chains: 15+ supported; pricing: subscription; API: GraphQL; sample: investigation graphs] |
| [Crystal Blockchain Analytics](https://crystalblockchain.com/products/) | Bitfury | (Product suite; 2024) Investigation and compliance tools for law enforcement and financial institutions.<br>[chains: 10+ supported; pricing: enterprise; integration: mature] |

---

### Sanctions & Watchlist Screening

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Refinitiv World-Check One](https://www.refinitiv.com/en/products/world-check-one) | Refinitiv | (Product docs; 2024) Comprehensive sanctions, PEP, and adverse media screening platform.<br>[pricing: per search; API: REST; sample: match_strength, risk_category] |
| [ComplyAdvantage AML Screening](https://complyadvantage.com/solutions/aml-screening/) | ComplyAdvantage | (Platform; 2024) AI-powered AML screening with real-time risk assessment and monitoring.<br>[pricing: subscription; API: REST; sample: risk_level, alert_categories] |
| [Dow Jones Risk & Compliance](https://professional.dowjones.com/risk/solutions/) | Dow Jones | (Solution suite; 2024) Third-party risk management and compliance screening solutions.<br>[pricing: enterprise; API: SOAP/REST; integration: banking systems] |

---

### All-in-One Compliance Platforms

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Sumsub AML Platform](https://sumsub.com/aml-platform/) | Sumsub | (Platform overview; 2024) End-to-end AML compliance with KYC, transaction monitoring, and case management.<br>[chains: major cryptocurrencies; pricing: per verification + monthly; API: REST; sample: applicant_status, risk_level] |
| [Shufti Pro Identity Verification](https://shuftipro.com/products/) | Shufti Pro | (Product suite; 2024) Identity verification, AML screening, and fraud prevention services.<br>[pricing: pay-per-use; API: REST; sample: verification_result, confidence_score] |


## 8. Repos & Example Integrations (Starter Kits)

### Open Source Tools

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [AML-Toolkit](https://github.com/bitcoin-tools/aml-toolkit) | Bitcoin-Tools | (GitHub repo; 2023) Bitcoin address clustering and transaction analysis scripts.<br>[maintained: partially; examples: clustering algorithms] |
| [Blockchain Parser](https://github.com/citp/BlockSci) | BlockSci | (GitHub repo; 2022) High-performance blockchain analysis platform for research and investigation.<br>[maintained: community; examples: address clustering, transaction graphs] |
| [Crystal Ball Analytics](https://github.com/OpenZeppelin/crystal-ball) | OpenZeppelin | (GitHub repo; 2024) Ethereum transaction analysis and smart contract security toolkit.<br>[maintained: active; examples: DeFi protocol analysis] |
| [ethereum-etl (blockchain-etl)](https://github.com/blockchain-etl/ethereum-etl) | GitHub | (Repo; 2018→maintained) ETL for blocks, transactions, logs, and smart-contract data extraction.<br>[note: MIT license] |
| [TRISA (Travel Rule)](https://github.com/trisacrypto/trisa) | GitHub / TRISA | (Repo; 2020→maintained) Reference TRISA implementation and testnet for Travel Rule messaging.<br>[note: MIT license] |
| [GraphSense (open-source)](https://github.com/graphsense) | GitHub / GraphSense | (Repo; active) Tools and dashboard for blockchain graph analytics.<br>[note: MIT license] |

---

### Integration Examples

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Chainalysis KYT Integration](https://github.com/chainalysis/kyt-python-sdk) | Sample Code | (SDK; 2024) Python SDK for Chainalysis KYT API with transaction monitoring examples.<br>[maintained: official; examples: real-time screening] |
| [Elliptic API Wrapper](https://github.com/elliptic-dev/api-wrapper) | Community | (Community repo; 2023) Unofficial Node.js wrapper for Elliptic API with compliance workflows.<br>[maintained: community; examples: address screening] |
| [OFAC Sanctions Checker](https://github.com/compliance-tools/ofac-checker) | Compliance Tools | (GitHub repo; 2024) Automated OFAC sanctions list checking with webhook notifications.<br>[maintained: active; examples: daily screening automation] |

---

### SAR Automation Templates

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [SAR Filing Automation](https://github.com/fintech-tools/sar-automation) | FinTech-Tools | (GitHub repo; 2023) Automated suspicious activity report generation and filing workflows.<br>[maintained: partially; examples: SAR narrative templates] |
| [AML Case Management](https://github.com/open-compliance/aml-case-mgmt) | Open-Compliance | (GitHub repo; 2024) Open source case management system for AML investigations.<br>[maintained: active; examples: alert triage workflows] |



## 9. Security Audits, Postmortems & Case Studies

### Exchange Hacks & AML Failures

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Binance Anti-Money Laundering Failures](https://www.reuters.com/investigates/special-report/fintech-crypto-binance-money/) | Reuters Investigation | (Investigative journalism; 2023) Investigation into Binance's AML control failures and regulatory enforcement actions. |
| [BitMEX AML Violations](https://www.cftc.gov/PressRoom/PressReleases/8369-21) | CFTC Enforcement | (Enforcement action; 2021) CFTC civil monetary penalty against BitMEX for AML program failures. |
| [Liberty Reserve Money Laundering](https://www.justice.gov/opa/pr/manhattan-us-attorney-announces-charges-against-operators-liberty-reserve) | DOJ Case Study | (DOJ press release; 2013) $6 billion virtual currency money laundering prosecution case study. |
| [Wormhole exploit postmortem & recovery notes](https://blog.jumpcrypto.com/wormhole-incident/) | Jump Crypto / Wormhole | (Case Study; 2022) Deep dive into Wormhole exploit, mitigation and recovery. [note: postmortem blog] |
| [Poly Network post-incident write-up](https://www.poly.network/) | Poly Network / community analysis | (Case Study; 2021) Exploit timeline and remediation steps. [note: blog / updates] |
| [FTX collapse](https://www.justice.gov/usao-sdny/pr/company-and-former-ceo-sentenced-related-ftx) | DOJ / SEC filings | (Enforcement; 2024) Example of enforcement, asset tracing and cross-jurisdiction investigations. [note: official releases] |

---

### Compliance Program Audits

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Coinbase AML Assessment](https://www.dfs.ny.gov/reports_and_publications/press_releases/pr202107141) | NY DFS | (Regulatory assessment; 2021) NY DFS assessment of Coinbase's BSA/AML compliance program effectiveness. |
| [Crypto Exchange Compliance Review](https://www.finra.org/rules-guidance/notices/21-18) | FINRA | (Regulatory notice; 2021) FINRA guidance on digital asset compliance for broker-dealers and funding portals. |

---

### Remediation Best Practices

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [AML Remediation Framework](https://advisory.kpmg.us/articles/2019/aml-remediation-framework.html) | KPMG | (Industry guide; 2019) Framework for remediating AML program deficiencies and regulatory violations. |
| [Wells Fargo AML Consent Order](https://www.occ.gov/news-issuances/news-releases/2020/nr-occ-2020-98.html) | OCC | (Consent order; 2020) OCC consent order requiring comprehensive AML program overhaul with lessons learned. |


## 10. Datasets, Benchmarks & Labelled Incidents

### Academic Datasets

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Elliptic Bitcoin Dataset](https://www.kaggle.com/ellipticco/elliptic-data-set) | Cambridge | (Research dataset; 2019) Labeled Bitcoin transaction dataset for illicit activity classification research. [access: Kaggle account required] |
| [Bitcoin Heist Dataset](https://archive.ics.uci.edu/ml/datasets/BitcoinHeistRansomwareAddressDataset) | UCI ML Repository | (ML dataset; 2020) Bitcoin addresses associated with ransomware payments for classification tasks. [access: public] |
| [Ethereum Fraud Detection Dataset](https://xblock.pro/ethereum-fraud-detection/) | Xblock | (Research dataset; 2021) Labeled Ethereum addresses for fraud detection machine learning models. [access: research license] |

---

### On-Chain Analytics Queries

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Dune Analytics AML Dashboards](https://dune.com/browse/dashboards?q=aml) | Dune Community | (Public dashboards; 2024) Community-created dashboards tracking suspicious cryptocurrency activity patterns. [access: free tier available] |
| [Chainalysis Public Data](https://public.chainalysis.com/) | Chainalysis | (Public portal; 2024) Publicly available cryptocurrency crime statistics and market analysis reports. [access: free registration] |
| [CoinMetrics Network Data](https://coinmetrics.io/community-network-data/) | Coin Metrics | (Public dataset; 2024) Community access to blockchain network data and on-chain metrics. [access: API key required] |

---

### Incident Databases

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [CipherTrace Cryptocurrency Crime Report](https://ciphertrace.com/cryptocurrency-crime-and-anti-money-laundering-report/) | Mastercard | (Annual report; 2024) Annual cryptocurrency crime statistics and AML trend analysis. [access: registration required] |
| [Crystal Blockchain Crime Reports](https://crystalblockchain.com/reports/) | Bitfury | (Research reports; 2024) Quarterly cryptocurrency crime analysis and investigation case studies. [access: free download] |

## 11. Privacy, Data Retention & GDPR Interplay

### Data Protection Framework

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [GDPR Article 6 Lawful Basis](https://gdpr-info.eu/art-6-gdpr/) | European Commission | (EU regulation; 2018) Legal basis for processing personal data in AML compliance contexts. [retention: varies by basis] |
| [ICO AML Data Processing Guidance](https://ico.org.uk/for-organisations/guide-to-data-protection/guide-to-the-general-data-protection-regulation-gdpr/lawful-basis-for-processing/public-task/) | UK ICO | (Official guidance; 2023) Data protection guidance for AML compliance processing under public task basis. |
| [EDPB Guidelines on Automated Decision-Making](https://edpb.europa.eu/our-work-tools/documents/public-consultations/2022/guidelines-082022-use-personal-data-scientific_en) | EDPB | (Official guidance; 2022) Guidelines on automated AML screening and profiling under GDPR. [retention: 6 years minimum AML] |

---

### Cross-Border Data Transfers

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Standard Contractual Clauses](https://ec.europa.eu/info/law/law-topic/data-protection/international-dimension-data-protection/standard-contractual-clauses-scc_en) | European Commission | (Legal instrument; 2021) SCCs for international AML data transfers to third countries. [legal basis: adequacy decisions] |
| [UK GDPR International Transfers](https://ico.org.uk/for-organisations/guide-to-data-protection/guide-to-the-general-data-protection-regulation-gdpr/international-transfers/) | UK ICO | (Official guidance; 2024) Post-Brexit data transfer mechanisms for AML compliance operations. |
| [CCPA and AML Compliance](https://oag.ca.gov/privacy/ccpa) | California AG | (State regulation; 2020) California Consumer Privacy Act implications for AML data processing. [retention: business purpose limitation] |

---

### Vendor Data Processing

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Chainalysis Privacy Policy](https://www.chainalysis.com/privacy-policy/) | Chainalysis | (Privacy policy; 2024) Data processing terms and retention periods for KYT services. [retention: varies by service] |
| [Elliptic Data Processing Agreement](https://www.elliptic.co/privacy-policy) | Elliptic | (DPA; 2024) GDPR-compliant data processing agreement for compliance services. [cross-border: UK-EU adequacy] |



## 12. Operational Playbooks & SOPs (How Teams Should Operate)

### SAR Filing Procedures

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [SAR Filing Instructions](https://www.fincen.gov/sites/default/files/shared/FinCEN_SAR_Electronic_Filing_Instructions.pdf) | FinCEN | (Official instructions; 2023) Step-by-step SAR electronic filing procedures and requirements. [note: regulator template] |
| [BSA E-Filing System](https://bsaefiling.fincen.treas.gov/main.html) | FinCEN | (Filing system; 2024) Official portal for BSA report submissions with user guides and technical specifications. |
| [Suspicious Activity Monitoring Playbook](https://www.acams.org/aml-white-paper-library/) | ACAMS | (Industry playbook; 2024) Alert investigation procedures and escalation workflows for AML teams. [note: membership required] |

---

### Investigation Workflows

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [AML Investigation Checklist](https://www.ffiec.gov/bsa_aml_infobase/pages_manual/olm_017.htm) | FFIEC | (Regulatory guidance; 2023) Standardized investigation procedures for suspicious activity cases. [note: template format] |
| [Case Management Best Practices](https://www.int-comp.org/careers/the-compliance-library/) | ICA | (Industry guide; 2024) AML case management workflows and documentation standards. [access: member resources] |
| [Alert Triage Framework](https://www.pwc.com/us/en/services/consulting/cybersecurity-privacy-forensics/financial-crimes/anti-money-laundering.html) | PwC | (Consulting framework; 2023) Risk-based alert prioritization and resource allocation methodology. [note: vendor playbook] |

---

### Training & Certification

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [AML Training Requirements](https://www.finra.org/rules-guidance/rulebooks/finra-rules/3310) | FINRA | (Regulatory requirement; 2024) Annual AML training requirements for registered persons and compliance staff. |
| [CAMS Certification Study Guide](https://www.acams.org/en/cams-certification) | ACAMS | (Certification program; 2024) Certified Anti-Money Laundering Specialist certification and study materials. [note: exam fee required] |
| [Wolfsberg Training Standards](https://www.wolfsberg-principles.com/articles/wolfsberg-aml-guidance-papers) | Wolfsberg Group | (Industry standards; 2023) AML training standards and competency frameworks for financial institutions. |

---

### Escalation & Governance

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Three Lines of Defense Model](https://www.theiia.org/en/content/position-papers/2020/the-iias-three-lines-model-an-update-of-the-three-lines-of-defense/) | IIA | (Governance framework; 2020) Risk management and compliance governance structure for AML programs. [note: template framework] |
| [AML Officer Responsibilities](https://www.fincen.gov/resources/advisories/fincen-advisory-fin-2019-a003) | FinCEN | (Official advisory; 2019) BSA compliance officer duties and regulatory expectations for program oversight. |



## 13. Testing, Simulation & QA

### Synthetic Data Generation

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [AML Testing Framework](https://www.protiviti.com/us-en/risk-compliance/anti-money-laundering-aml) | Protiviti | (Testing methodology; 2023) Comprehensive AML control testing procedures and validation frameworks. [note: consulting methodology] |
| [Transaction Monitoring Testing](https://advisory.kpmg.us/articles/2020/transaction-monitoring-testing.html) | KPMG | (Industry guide; 2020) Statistical sampling and backtesting methodologies for TM rule validation. [note: privacy considerations] |
| [Synthetic Data for AML](https://mostly.ai/synthetic-data-use-cases/financial-services) | Mostly AI | (Technical solution; 2024) Privacy-preserving synthetic transaction data generation for model training. [pricing: enterprise] |

---

### Model Validation & Backtesting

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Model Risk Management](https://www.federalreserve.gov/supervisionreg/srletters/sr1107a1.pdf) | Federal Reserve | (Regulatory guidance; 2011) SR 11-7 model risk management guidance applicable to AML scoring models. [note: foundational guidance] |
| [AML Model Validation](https://www2.deloitte.com/us/en/pages/regulatory/articles/aml-model-validation-governance.html) | Deloitte | (Industry practice; 2022) Independent validation procedures for machine learning AML models. [note: governance framework] |

---

### Load Testing & Performance

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Apache JMeter Load Testing](https://jmeter.apache.org/usermanual/get-started.html) | Apache Foundation | (Open source tool; 2024) Load testing framework for transaction monitoring system performance validation. [note: includes scripts] |
| [Kubernetes Monitoring](https://prometheus.io/docs/introduction/overview/) | Prometheus | (Monitoring platform; 2024) Infrastructure monitoring for real-time AML processing pipelines and alerting. [note: open source] |


## 14. Research Gaps & Open Questions

### Technical Research Needs

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Cross-Chain Attribution Challenges](https://dci.mit.edu/research/2023/3/1/cross-chain-investigation-challenges) | MIT DCI | (Research paper; 2023) Open problems in multi-blockchain transaction tracing and attribution accuracy. [research gap: cross-chain bridges] |
| [Privacy Coin Compliance](https://www.rand.org/pubs/research_reports/RRA465-1.html) | RAND Corporation | (Policy research; 2020) Regulatory challenges for privacy-enhanced cryptocurrencies and compliance feasibility. [research gap: technical vs regulatory balance] |
| [DeFi Compliance Framework](https://www.imf.org/en/Publications/WP/Issues/2021/01/29/Regulating-the-Crypto-Ecosystem-The-Case-of-Stablecoins-and-Arrangements-50074) | IMF Working Paper | (Academic research; 2021) Regulatory framework gaps for decentralized finance protocols and smart contracts. |

---

### Dataset & Labeling Needs

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Blockchain Annotation Project](https://blog.chainalysis.com/reports/blockchain-analysis-accuracy-precision/) | Chainalysis | (Industry research; 2022) Call for standardized blockchain address labeling and ground truth datasets. [opportunity: collaborative labeling] |
| [AML AI Bias Research](https://www.brookings.edu/research/algorithmic-bias-detection-and-mitigation/) | Brookings | (Policy research; 2021) Research needs for bias detection and fairness in automated AML decision systems. [research gap: algorithmic fairness] |

---

### Regulatory Evolution

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Central Bank Digital Currency AML](https://www.bis.org/publ/othp42.htm) | BIS | (Policy paper; 2021) AML/CFT implications of central bank digital currencies and programmable money. [research gap: CBDC compliance design] |
| [Travel Rule Technical Implementation](https://www.fatf-gafi.org/en/publications/Fatfrecommendations/Virtual-assets-VASP-travel-rule.html) | FATF | (Implementation guide; 2023) Technical standards development needs for travel rule interoperability. [standardization opportunity: messaging protocols] |


## 15. Community & Standards (Working Groups, RFCs)

### Industry Working Groups

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [FATF Virtual Assets Working Group](https://www.fatf-gafi.org/en/topics/Virtual-assets.html) | FATF-GAFI | (Working group; 2024) International policy development for virtual asset regulation and standards. [participation: government delegates] |
| [Global Digital Finance AML Working Group](https://www.gdf.io/workstreams/) | GDF | (Industry consortium; 2024) Industry self-regulatory standards development for digital asset compliance. [participation: membership based] |
| [Blockchain Association Policy Committee](https://theblockchainassociation.org/policy-committees/) | Blockchain Association | (Trade association; 2024) US cryptocurrency industry policy advocacy and regulatory engagement. [participation: member companies] |

---

### Technical Standards Development

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [InterVASP Travel Rule Protocol](https://openvasp.org/) | OpenVASP | (Technical standard; 2024) Open protocol for FATF travel rule implementation and VASP interoperability. [participation: open source contributors] |
| [TRISA Travel Rule Protocol](https://trisa.io/) | TRISA | (Technical implementation; 2024) Travel Rule Information Sharing Architecture for secure VASP messaging. [participation: VASP implementation] |
| [Financial Data Exchange](https://financialdataexchange.org/) | FDX | (API standard; 2024) Standardized APIs for financial data sharing including compliance data exchange. [participation: FI membership] |

---

### Research Communities

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [Financial Cryptography Conference](https://fc24.ifca.ai/) | IACR | (Academic conference; 2024) Premier academic venue for cryptocurrency and financial technology security research. [participation: paper submission/attendance] |
| [Cryptocurrency Research Discord](https://discord.gg/cryptocurrency-research) | Academic Community | (Community forum; 2024) Academic and industry researchers discussing blockchain analysis and compliance. [participation: Discord invite] |
| [DeFi Security Summit](https://defisecuritysummit.org/) | Community Event | (Industry conference; 2024) Annual gathering focusing on DeFi security, compliance, and risk management. [participation: registration] |

---

### Professional Networks

| Title | Author / Source | Why include |
| :--- | :--- | :--- |
| [ACAMS Chapter Events](https://www.acams.org/en/chapters) | ACAMS | (Professional network; 2024) Regional chapter meetings and networking events for AML professionals. [participation: membership] |
| [ICA Compliance Community](https://www.int-comp.org/) | International Compliance Association | (Professional body; 2024) Global compliance professional association with AML specialization tracks. [participation: membership] |
| [Wolfsberg Group](https://www.wolfsberg-principles.com/) | Wolfsberg | (Industry group; 2024) Leading banks collaboration on AML/CFT standards and best practices. [participation: invitation only] |








## Contributing Guidelines

Content Quality Standards: 

- All links must be tested and accessible
- Include archive.org backup for critical historical documents
- Mark paywalled content clearly in notes section
- Verify jurisdictional scope and legal authority
- Update "last_checked" metadata quarterly


### Submission Process

Fork repository and create feature branch
Add links following exact template format
Test all URLs and verify content accuracy
Update metadata and last_updated timestamp
Submit pull request with detailed description
Respond to reviewer feedback within 7 days


### License & Disclaimer
This resource is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0). Content is for educational and informational purposes only. Always consult qualified legal counsel for specific compliance requirements.

### Disclaimer: 

Regulatory requirements change frequently. Verify current requirements with appropriate authorities. Contributors are not responsible for the accuracy, completeness, or currency of external resources.

Last Updated: August 26, 2025
Maintainer: cryptowithshashisupport@gmail.com
Contributors: 0
