\# Crypto News Aggregator Dataset



This repository contains a curated dataset of \*\*crypto news aggregator websites\*\*, focused strictly on platforms that aggregate news from multiple sources.



\---



\## 📌 Scope



This dataset includes only \*\*true news aggregators\*\*, defined as sites that:



\* Aggregate crypto news, headlines, or article links

\* Pull content from multiple external publishers

\* Function as a discovery layer for crypto news



\---



\## ❌ Excluded



The following types are intentionally excluded:



\* On-chain analytics platforms (e.g. Nansen, DeFiLlama)

\* Trading dashboards (DEX Screener, GeckoTerminal)

\* Social sentiment tools (LunarCrush, Santiment)

\* Single-source news sites (CoinDesk-style publishers)

\* Exchange-owned news pages



\---



\## 📂 Structure



input/

seed\_sites.csv



output/

final\_news\_aggregators\_v3.csv

news\_aggregators\_additional\_20.csv



.gitignore



\---



\## 📊 Dataset Columns



Each entry includes:



\* website\_name → Name of the platform

\* homepage\_url → Main URL

\* category → Type of aggregator:



&#x20; \* news\_aggregator

&#x20; \* headline\_feed

&#x20; \* news\_discovery

&#x20; \* hybrid\_news\_aggregator

\* why\_similar → Explanation of aggregation behavior

\* confidence → Quality score:



&#x20; \* high

&#x20; \* medium



\---



\## 🧠 Methodology



1\. Start with seed aggregator sites

2\. Expand using AI-assisted discovery (Codex)

3\. Filter strictly for news aggregation behavior

4\. Remove:



&#x20;  \* duplicates

&#x20;  \* non-news aggregators

&#x20;  \* low-confidence entries

5\. Normalize structure and categories



\---



\## 🎯 Use Cases



This dataset can be used for:



\* Crypto news tracking

\* Content research and idea discovery

\* SEO analysis (news sources)

\* Building aggregation tools or bots



\---



\## ⚠️ Notes



\* Dataset prioritizes precision over size

\* Only sites that clearly match the definition are included

\* Some borderline platforms are intentionally excluded



\---



\## 🔄 Future Improvements



\* Expand with additional verified aggregators

\* Add RSS/feed availability

\* Categorize by use case (breaking news, narrative tracking, etc.)



