# -Cross-Linguistic-Analysis-of-Financial-News-Coverage


## 📌 Project Overview

This project investigates how financial news coverage varies between English and Chinese-language media from 2007 to 2021. Using a bilingual parallel corpus of financial articles originally published by Hung et al. (2021), we explore how language and culture influence discourse surrounding global economic topics such as **inflation**, **tariffs**, **AI**, and **labor costs**.

Our central research question is:

> **How do language and culture influence the representation and coverage of financial events in English versus Chinese media?**

---

## 🧰 Methodology

We employed a suite of text mining and clustering techniques to explore the corpus. Articles were processed and analyzed using consistent methods across both languages to uncover patterns, sentiment trends, and editorial priorities. Our eight main analytical modules were:

### 1. Preprocessing and Tokenization
- English text: Lowercased, punctuation removed, stop words filtered.
- Chinese text: Regex used to remove non-Chinese characters and punctuation.
- Tokenization allowed compatibility with TF-IDF, LDA, and other NLP tools.

### 2. Word/Character Frequency Analysis
- Used the `Counter` module to identify high-frequency financial terms.
- Enabled cross-linguistic comparison of dominant financial vocabulary.

### 3. Temporal Trend Analysis
- Grouped articles by year.
- Tracked term frequency of key words like "crisis", “股票”, and “市场”.
- Visualized temporal shifts in financial discourse.

### 4. Event Spike Detection
- Computed daily article counts and identified volume spikes beyond the 95th percentile.
- Sampled article titles from high-volume days to identify real-world financial events.

### 5. Cross-Cultural Keyword Coverage
- Compared frequency of parallel financial terms across corpora.
- Created heatmaps and bar charts to visualize disparities in term emphasis.

### 6. Article Structure Analysis
- Compared paragraph count, word count, and character count.
- Assessed translation consistency and structural alignment between languages.

### 7. Topic Modeling (TF-IDF + LDA)
- Applied TF-IDF to convert English articles into feature vectors.
- Used LDA to discover 8 latent themes related to banking, trade, recession, etc.

### 8. Time-Based Event Clustering
- Grouped articles by week.
- Identified 90th-percentile spikes in volume.
- Extracted titles to investigate causes behind these bursts.

---

## 📈 Key Findings

- **Thematic Emphasis**:
  - English articles emphasized **crisis** and **banking instability** (e.g., 2008, 2020).
  - Chinese articles focused more on **investment** and **growth**.

- **Editorial Priorities**:
  - Chinese media showed stronger alignment with **policy and government messaging**.
  - English media highlighted **market dynamics** and **recession narratives**.

- **Narrative Structures**:
  - Chinese articles had **shorter paragraphs** and **more compressed styles**.
  - Structural differences reflected distinct journalistic conventions.

- **Temporal Patterns**:
  - 124 major events were identified with **synchronized bursts** of coverage.
  - Examples: 2008 global financial crisis, US-China trade tensions.

---

## 🔬 Limitations

- **Sentiment Analysis**:
  - Tools like VADER are English-optimized; Chinese sentiment pipelines were limited.
  - Chinese texts were not translated to preserve linguistic authenticity.

- **Topic Modeling Disparities**:
  - Lack of aligned Chinese topic models limited direct comparison.
  - Keyword-based methods may miss subtleties such as irony or metaphor.

---

## 🚀 Future Work

To build on this research:
- Implement multilingual topic models (e.g., BERTopic with transformer embeddings).
- Improve Chinese-language sentiment analysis tools.
- Analyze multimedia financial reporting (e.g., headlines + visuals).
- Extend the corpus to include post-COVID financial narratives.

---

## 📊 Sample Visualization

**Figure 1: Temporal Trends of Key Financial Terms (2005–2021)**  
This line chart compares the usage of "crisis", "market", and "investment" over time in both languages. Notable trends:
- Spikes in “crisis” in English articles during 2008 and 2020.
- Chinese articles consistently emphasized “investment” and “市场” (market).

---

## 📚 Citation

Hung, J., et al. (2021). *Parallel Bilingual Financial News Dataset (2007–2021)*. Journal of Open Humanities Data. https://doi.org/10.5334/johd.XX
