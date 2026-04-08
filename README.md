# Crypto News Aggregator Dataset

A curated dataset of **crypto news aggregator websites**.

This repository focuses strictly on platforms that **aggregate news from multiple sources**, helping you track narratives, headlines, and market-moving events in one place.

---

## What this dataset is

Instead of collecting random crypto websites, this dataset is built to answer one question:

> **Where can you see crypto news aggregated across multiple sources in real-time?**

Each entry is selected based on its ability to:

* Aggregate crypto news or headlines
* Pull content from multiple publishers
* Function as a discovery layer for news

---

## How it works

The dataset is built using a structured pipeline:

1. Start with seed aggregator sites
2. Expand using AI-assisted discovery (Codex)
3. Apply strict filtering:

   * remove dashboards, analytics tools, and trading platforms
   * remove single-source editorial sites
4. Deduplicate and normalize
5. Keep only **high-confidence news aggregators**

This ensures the dataset prioritizes:

> **precision over volume**

---

## What is NOT included

To keep the dataset clean, the following are excluded:

* On-chain analytics platforms (Nansen, DeFiLlama)
* Trading dashboards (DEX Screener, GeckoTerminal)
* Social sentiment tools (LunarCrush, Santiment)
* Single-source publishers (CoinDesk-style sites)
* Exchange-owned news pages

---

## Repository structure

input/
seed_sites.csv

output/
final_news_aggregators_v3.csv
news_aggregators_additional_20.csv

.gitignore
README.md

---

## Dataset format

Each row includes:

* **website_name** → Platform name
* **homepage_url** → Main URL
* **category** → Aggregator type:

  * news_aggregator
  * headline_feed
  * news_discovery
  * hybrid_news_aggregator
* **why_similar** → Why it qualifies
* **confidence** → Quality level:

  * high
  * medium

---

## How to use this dataset

You can use this dataset to:

* Track crypto news across multiple sources
* Discover narratives early
* Find content ideas
* Build news aggregation tools or bots

A simple workflow:

1. Open top aggregator sites
2. Scan headlines daily
3. Identify repeating narratives
4. Turn them into content or insights

---

## Notes

* This dataset is intentionally **small but clean**
* Only sites that clearly match the definition are included
* Borderline platforms are excluded on purpose

---

## Future improvements

* Add more verified news aggregators
* Include RSS/feed availability
* Rank aggregators by usefulness
* Build automated tracking pipelines
