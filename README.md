# 🔬 IP Intelligence Tools

<div align="center">

![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

**A suite of open-source tools for patent search, portfolio management, and IP intelligence.**

</div>

---

## The Problem With Patent Data

Patent intelligence workflows typically require three things that don't come together easily:

1. **Discovery** — finding what exists across jurisdictions, by competitor, by technology area
2. **Portfolio management** — tracking your own filings, statuses, and family relationships
3. **Translation** — turning dense patent language into something a business team can actually use

Most tools do one of these. This suite does all three.

---

## The Workflow

```
                    ┌─────────────────────────────┐
                    │       patent-scraper        │
                    │                             │
                    │  Search any assignee across │
                    │  US, WO, EP, JP, CN & more  │
                    │  → structured Excel output  │
                    └──────────────┬──────────────┘
                                   │
                        Discovery & landscape
                        Competitive intelligence
                        Prior art research
                                   │
                                   ▼
                    ┌─────────────────────────────┐
                    │     patent-lookup-tool      │
                    │                             │
                    │  Enrich your own portfolio  │
                    │  with live GP data + AI     │
                    │  invention summaries        │
                    └─────────────────────────────┘
                                   │
                        Portfolio tracking
                        Family aggregation
                        Plain-English summaries
                        Licensing one-pagers
```

---

## The Tools

### 🔭 [patent-scraper](https://github.com/elichter/patent-scraper)

> *Who's filing what — and where?*

Search any assignee across global patent systems and pull structured, analysis-ready data. Built for competitive intelligence, prior art research, and technology landscape analysis.

**Best for:**
- Monitoring a competitor's R&D pipeline
- Building a patent landscape for a technology area
- Prior art searches across jurisdictions
- Tracking filing trends over time

**Highlights:**
- Searches US, WO, EP, JP, CN and more via SerpAPI + Google Patents
- Deduplicates records across jurisdictions
- Interactive assignee review step catches false positives
- Downstream analytics: grants by year, co-assignees, jurisdiction heatmaps, word clouds, t-SNE clustering
- Parallel fetch for large portfolios

---

### 📋 [patent-lookup-tool](https://github.com/elichter/patent-lookup-tool)

> *What do we have — and what does it mean?*

Takes your own patent portfolio spreadsheet and enriches it with live data from Google Patents and EPO, then generates AI-powered plain-English summaries of every invention.

**Best for:**
- Tech transfer offices tracking their portfolio
- IP counsel auditing a client's filings
- Researchers documenting innovation outputs
- Licensing teams preparing outreach materials

**Highlights:**
- Handles US utility, design (29/xxx), and PCT/WO filings
- Groups filings into patent families with aggregated dates and statuses
- AI-generated technical + plain-English invention summaries — no prompting required
- Data quality flags: detects wrong patents, title mismatches, provisional-only families
- Color-coded two-sheet Excel output

---

## Combined Use

The two tools are designed to work together:

1. Use **patent-scraper** to pull a competitor's full filing history → identify technology gaps or licensing opportunities
2. Use **patent-lookup-tool** on your own portfolio → understand what you have relative to what you found
3. Export both to Excel → compare side by side for strategic analysis

---

## Getting Started

Each tool has its own installation instructions and configuration:

- → **[patent-scraper README](https://github.com/elichter/patent-scraper)**
- → **[patent-lookup-tool README](https://github.com/elichter/patent-lookup-tool)**

Both tools auto-detect missing dependencies and offer to install them on first run.

---

## License

Both tools are released under the [MIT License](https://opensource.org/licenses/MIT).

---

<div align="center">
<i>Built for IP teams who want intelligence, not just data.</i>
</div>
