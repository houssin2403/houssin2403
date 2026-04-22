<div align="center">

```
██╗  ██╗ ██████╗ ██╗   ██╗███████╗███████╗██╗███╗   ██╗    ██████╗ ██████╗ ██╗███████╗
██║  ██║██╔═══██╗██║   ██║██╔════╝██╔════╝██║████╗  ██║    ██╔══██╗██╔══██╗██║██╔════╝
███████║██║   ██║██║   ██║███████╗███████╗██║██╔██╗ ██║    ██║  ██║██████╔╝██║███████╗
██╔══██║██║   ██║██║   ██║╚════██║╚════██║██║██║╚██╗██║    ██║  ██║██╔══██╗██║╚════██║
██║  ██║╚██████╔╝╚██████╔╝███████║███████║██║██║ ╚████║    ██████╔╝██║  ██║██║███████║
╚═╝  ╚═╝ ╚═════╝  ╚═════╝ ╚══════╝╚══════╝╚═╝╚═╝  ╚═══╝    ╚═════╝ ╚═╝  ╚═╝╚═╝╚══════╝
```

### Data Specialist · Growth Engineer · Futur MSc Data Science

*Building data pipelines and growth systems that ship — not just notebooks.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/houssin-dris)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat&logo=vercel&logoColor=white)](https://houssin-dris.dev)
[![3ersi.com](https://img.shields.io/badge/3ersi.com-6C63FF?style=flat&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iMTAiIHN0cm9rZT0id2hpdGUiIHN0cm9rZS13aWR0aD0iMiIgZmlsbD0ibm9uZSIvPjwvc3ZnPg==&logoColor=white)](https://3ersi.com)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:houssindris2403@gmail.com)

</div>

---

## `$ whoami`

```python
houssin = {
    "role"       : "Data Growth Specialist @ Yucca Labs",
    "location"   : "Lyon, France 🇫🇷  ·  Algeria 🇩🇿",
    "languages"  : ["French (native)", "Arabic (native)", "English (working)"],
    "focus"      : ["Data Engineering", "AI Orchestration", "SEO Analytics", "Growth"],
    "studying"   : "Applied Mathematics L3 → MSc Data Science (2026)",
    "shipped"    : "211+ venue records · 14 wilayas · 6 custom Python scripts",
}
```

I don't just analyze data — I build the systems that collect it, clean it, enrich it, and turn it into business growth. My work lives at the intersection of **Python automation**, **LLM orchestration**, and **SEO technical strategy**.

Currently operating the full data pipeline for **[3ersi.com](https://3ersi.com)** — Algeria's wedding vendor platform.

---

## `$ ls ./projects --sort=impact`

### 🏗️ [National ETL Pipeline — 3ersi.com](./pipeline-3ersi)
> *Scraped, cleaned and enriched 211+ wedding venues across 14 Algerian wilayas*

The full data engineering story: from raw Google Maps results to a production-ready trilingual database (FR/AR/EN) with GPS coordinates, verified phone numbers, Facebook pages, capacity estimates, and SEO descriptions — all automated.

```
Instant Scraper → Python merge → Claude AI cleanup → phone_add.py
→ fb_scraper.py → photo_scraper.py → image_format.py → SEO descriptions
```

**Stack:** `Python` `Pandas` `Playwright` `Google Maps API` `Google Drive API` `Claude AI`  
**Scale:** 211+ records · 14 wilayas · ~9 data fields per venue · FR/AR/EN

| Wilaya group | Venues | Status |
|---|---|---|
| Béjaïa + Tizi Ouzou + Boumerdès | 54 | ✅ Delivered |
| Tlemcen + Sétif + Batna | 45 | ✅ Delivered |
| Mostaganem + Tipaza + Annaba | 22 | ✅ Delivered |
| Oran + Constantine | 48 | 🔄 In review |
| Chlef + Médéa + Bouira | 42 | 🔄 In progress |

---

### 🤖 [AI Vision SEO Image Renamer](./seo-image-renamer)
> *Pipeline that semantically renames thousands of images using computer vision*

**The problem:** Thousands of images named `img-01.jpg`, `img-02.jpg` — zero SEO value.  
**The solution:** A 4-step pipeline that downloads images from Sheets, organizes them into slug-based folders, sends them to a Vision AI model to understand the visual content, then renames them with descriptive French keywords.

```
Google Sheets → JSON extraction → local download + folder structure
→ Vision AI analysis → semantic rename → Google Drive re-upload → new links back to Sheets
```

**Key engineering decision:** Built an incremental monitoring script that detects which folders failed processing and retargets only those — avoiding full reprocessing on crashes. Reduced wasted API calls by ~90%.

**Format:** `[article-slug]-[seo-description].jpg`  
e.g. `salle-setif-grande-salle-moderne-lumineuse.jpg`

---

### 📊 [SEO Audit & Growth Strategy — 3ersi.com](./seo-audit-3ersi)
> *Data-driven organic performance analysis using Google Search Console*

Comparative cohort analysis (Period A: 48 days vs Period B: 20 days) that uncovered a classic SEO paradox: **better rankings, stagnating CTR**.

**Diagnosis:** Structural URL cannibalization — dynamic search pages (`/recherche?wilaya=1&commune=34`) competing against each other in SERPs, diluting authority with no semantic value.

```
Raw GSC export → cohort analysis → cannibalization detection
→ prioritized action plan → implementation roadmap
```

| Metric | Period A | Period B | Delta |
|---|---|---|---|
| Avg. position | 8.12 | 6.83 | **−1.29 pts 🚀** |
| Impressions/day | 9,652 | 10,479 | +8.6% ✅ |
| Clicks/day | 244 | 259 | +5.9% ✅ |
| Global CTR | 2.53% | 2.47% | −0.06 pts ⚠️ |

**Roadmap delivered:**
- 🔴 Static landing pages per wilaya/commune (est. +20–40% CTR)
- 🔴 Title/Meta rewrite for high-impression, low-CTR pages (est. +15–25% clicks)
- 🟡 Internal linking push for pages at positions 11–15
- 🟡 LocalBusiness Schema Markup (est. +15–30% CTR via rich snippets)

---

### 🌍 [Community Architecture POC — 3ersi.com](./community-poc)
> *Product design for a UGC-driven community platform with a built-in data moat*

Designed the community layer of 3ersi.com: 50+ culturally-targeted seed topics across 5 categories, bilingual FR/AR architecture from day one, geographic structure across 58 wilayas, and a direct link between forum posts and vendor listings.

**The moat:** Local market surveys per wilaya (wedding hall prices, caterer costs, photographer rates) generate exclusive first-party data that international competitors can't replicate.

```
UGC post → linked to vendor listing → drives traffic + conversion
Local survey → exclusive market data → SEO longtail + monetization lever
```

---

### 🔧 [Digital Asset Normalizer](./asset-normalizer)
> *Bulk rename engine for SEO-compliant file naming at scale*

Strict transformation rules applied to thousands of files:
- Keep article slug as prefix
- Replace numeric suffix with SEO-descriptive content keyword
- Lowercase + hyphens only, no accents, no special characters
- Preserve `.jpg` extension and folder hierarchy

Zero broken links during migration. Zero manual intervention after setup.

---

## `$ cat ./stack.json`

```json
{
  "data_engineering" : ["Python", "Pandas", "ETL pipelines", "Web scraping"],
  "scraping"         : ["Playwright", "Scrapy", "Selenium", "Instant Data Scraper"],
  "ai_orchestration" : ["Claude 3 Vision", "Gemini Pro Vision", "LLM pipelines"],
  "analytics"        : ["Google Search Console", "Google Analytics 4", "Windsor.ai", "Power BI"],
  "apis"             : ["Google Drive API", "Google Sheets API", "Google Maps API"],
  "seo_technical"    : ["Schema Markup", "URL architecture", "Cannibalization audit", "CTR optimization"],
  "web_dev"          : ["React", "Vite", "Tailwind CSS", "Framer Motion"],
  "mathematics"      : ["Optimization", "Operational Research", "Statistics", "LaTeX"],
  "languages"        : ["French", "Arabic", "English"]
}
```

---

## `$ git log --oneline --graph`

```
* Pipeline V3: image_format.py — auto-crop + ratio uniformization       [Mar 10]
* Deploy: 9 wilayas complete · 121 venues delivered                     [Mar 24]
* Feature: incremental monitoring for Vision AI pipeline                [Mar 05]
* Feature: fb_scraper.py — Facebook page extraction                     [Mar 02]
* Feature: photo_scraper.py — Google Maps photo download + Drive upload [Mar 01]
* Fix: bypass Google Maps 10-result limit in maps_tools.py              [Feb 28]
* Init: Pipeline V1 — scraping + phone/maps matching (SheetV1→V3)       [Feb 26]
```

---

## `$ cat ./stats`

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=houssin-dris&show_icons=true&theme=dark&hide_border=true&bg_color=0a0a0f&title_color=a78bfa&icon_color=6c63ff&text_color=9090a8)
&nbsp;&nbsp;
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=houssin-dris&layout=compact&theme=dark&hide_border=true&bg_color=0a0a0f&title_color=a78bfa&text_color=9090a8)

</div>

---

## `$ cat ./currently`

```bash
$ python pipeline.py --wilaya oran constantine --status review
$ python clean.py --wilaya chlef medea bouira --status in_progress
$ research_applications --track "MSc Data Science" --year 2026
$ freelance --markets "Algeria, France" --stack "Python, React, Data"
```

---

<div align="center">

*"Don't just analyze data. Build the system."*

**Open to:** Freelance missions · Data engineering · Growth & SEO consulting · MSc collaborations

</div>
