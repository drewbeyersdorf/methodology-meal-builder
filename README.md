# Methodology Data Search

**Purpose:** Central hub for all GoMethodology.com data intelligence and analysis.

**Goal:** Build a clear picture of WHO and WHAT is gomethodology.com to support strategic decisions and the $600M exit target.

---

## Folder Structure

```
methodology_data_search/
│
├── 01_slack_data/              # Slack workspace intelligence
│   ├── CICADA-01_WORKSPACE_MAP/  # Complete workspace export (2,100+ files)
│   │   ├── PUBLIC/               # 187 public channels
│   │   ├── PRIVATE/              # 145 private channels
│   │   ├── GROUP_DMS/            # 1,365 group conversations
│   │   └── DIRECT_MESSAGES/      # 411 DM threads
│   ├── cicada.py                 # Main Slack discovery agent
│   ├── slack_client.py           # Slack API client
│   ├── extractors.py             # Topic/dependency extraction
│   ├── writers.py                # Markdown generation
│   ├── dead_channel_audit.py     # Channel vitality analysis
│   └── channel_consolidation_analysis.py
│
├── 02_google_drive_data/       # Google Drive exports & analysis
│   ├── Takeout/                  # Calendar, Chrome, Contacts
│   ├── Takeout 2/                # Drive (2,300+ files)
│   │   └── Drive/                # Financial docs, recipes, HR, vendors
│   ├── synergy_analysis_output/  # 12-layer bot analysis results
│   ├── synergy_bots/             # Analysis automation scripts
│   ├── STALE_DOCS_AUDIT.csv      # Document freshness report
│   └── Methodology OKRs Q4 2025.txt
│
├── 03_pgadmin_queries/         # PostgreSQL database queries
│   ├── 00_DATABASE_MAP.sql       # Schema discovery (RUN FIRST)
│   ├── 01_WHO_PEOPLE.sql         # People, teams, roles (pending)
│   ├── 02_WHAT_OPERATIONS.sql    # Products, orders, financials (pending)
│   ├── 03_STRATEGIC_INSIGHTS.sql # Needle-moving analytics (pending)
│   └── README.md                 # Query workflow guide
│
├── 04_fireflies_data/          # Meeting transcripts (when available)
│   └── README.md                 # Setup instructions
│
├── archive/                    # Historical analysis & teaching materials
│   ├── AI_TEACHING_CURRICULUM/
│   ├── CPO_CODE_LESSONS/
│   ├── diagrams_and_chef_work/
│   └── synergy-project/          # Original analysis scripts
│
├── .env                        # API keys (Slack, Google Gemini)
├── requirements.txt            # Python dependencies
├── analyze_portioning_photos.py  # AI food plating analysis
└── download_portioning_photos.py # Photo download utility
```

---

## Quick Start

### 1. Map the Database
```bash
# Open pgAdmin → Run 03_pgadmin_queries/00_DATABASE_MAP.sql
# Share results to build targeted queries
```

### 2. Explore Slack Data
```bash
# Key reports in 01_slack_data/CICADA-01_WORKSPACE_MAP/:
# - 00_EXECUTIVE_INDEX.md (start here)
# - PURE_FACTUAL_REPORT.md (32,580 lines of facts)
# - STRATEGIC_OVERLAY_REPORT.md (growth strategy)
```

### 3. Review Financial Data
```bash
# Key files in 02_google_drive_data/:
# - synergy_analysis_output/executive_financials.json
# - Takeout 2/Drive/ (P&L, COGS, vendor invoices)
```

---

## Key Metrics (from existing analysis)

| Metric | Value |
|--------|-------|
| Annual Revenue | $7.33M (2022 YTD) |
| Net Margin | 8.6% (low - industry 15-25%) |
| Slack Users | 1,061 |
| Slack Channels | 332 (187 public, 145 private) |
| Messages Analyzed | 126,165 |
| Chefs | 27+ |
| Exit Target | $600M |

---

## Data Sources

1. **Slack** - Workspace export via CICADA-01 agent
2. **Google Drive** - Takeout export (financials, recipes, HR, vendors)
3. **pgAdmin** - Company database (to be mapped)
4. **Fireflies** - Meeting transcripts (to be imported)
