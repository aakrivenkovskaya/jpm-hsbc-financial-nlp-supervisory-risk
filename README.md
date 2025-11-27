# Cambridge × Bank of England  
# Supervisory-Grade Financial NLP System**  
### **JP Morgan & HSBC Earnings Call Q&A Analysis (2023–2025)**

This repository presents a **supervisory-grade Financial NLP system** developed **on the University of Cambridge Data Science Programme**, in **analytical collaboration with senior practitioners from the Bank of England’s Prudential Regulation Authority (PRA)**.

The project applies advanced AI and NLP techniques to **JP Morgan** and **HSBC** quarterly earnings call Q&A transcripts, replicating analytical workflows used by central banks to identify:

- emerging prudential and market risks  
- transparency gaps and evasive answering  
- tone divergence between executives and analysts  
- discourse-based early-warning indicators  
- forward-looking supervisory concerns  

The system integrates **topic modelling, sentiment analysis, evasiveness detection, LLM-based supervisory summaries**, and an upcoming **AI Agent layer** for interactive risk intelligence.

---

## **1. Executive Summary**

Global systemically important banks (G-SIBs) provide critical forward-looking signals in their earnings call Q&A sessions.  
Supervisory teams use this discourse to understand:

- liquidity and funding pressures  
- narrative deviations from actual performance  
- tone asymmetries between managers and analysts  
- governance or conduct red flags  
- emerging risk themes aligned to PRA categories  

This project operationalises those workflows using state-of-the-art AI.

The result is an **end-to-end Financial NLP system** designed to support supervisory decision-making.

---

## **2. Project Context & Institutional Framework**

### **University of Cambridge**
This work originates from the University of Cambridge’s advanced Data Science Programme, focusing on high-trust, high-impact analytical use cases.

### **Bank of England · PRA Collaboration**
The analysis was carried out with **analytical input and supervisory framing provided by practitioners from the Bank of England’s Prudential Regulation Authority**.

Their insight influenced:

- risk-category mapping  
- evaluation of managerial tone  
- evasiveness identification  
- design of supervisory summaries  
- emphasis on forward-looking narratives  

### **Data from JP Morgan & HSBC**
The system analyses **real earnings call Q&A transcripts** from:

- **JP Morgan Chase**  
- **HSBC Holdings**

covering multiple quarters (2023–2025).

---

## **3. System Architecture**

        ┌──────────────────────────────────────────────────────────────┐
        │  1. Transcript Extraction & Pre-processing                   │
        │  Parsing → cleaning → metadata normalisation                 │
        └──────────────────────────────────────────────────────────────┘
                         │
                         ▼
        ┌──────────────────────────────────────────────────────────────┐
        │  2. Topic Modelling (BERTopic + Finance Embeddings)          │
        │  PRA-aligned themes & narrative trajectories                 │
        └──────────────────────────────────────────────────────────────┘
                         │
                         ▼
        ┌──────────────────────────────────────────────────────────────┐
        │  3. Sentiment Analysis (Fine-tuned DistilRoBERTa)            │
        │  Manager vs Analyst divergence                               │
        └──────────────────────────────────────────────────────────────┘
                         │
                         ▼
        ┌──────────────────────────────────────────────────────────────┐
        │  4. Evasion Detection (DeBERTa NLI + RoBERTa Ranking)        │
        │  Transparency red flags                                      │
        └──────────────────────────────────────────────────────────────┘
                         │
                         ▼
        ┌──────────────────────────────────────────────────────────────┐
        │  5. Supervisory Summaries (LLM-generated, GPT-4.1)           │
        │  Forward-looking PRA-aligned briefings                       │
        └──────────────────────────────────────────────────────────────┘
---

## **4. Repository Structure**

notebooks/
01_data_preparation_and_extraction.ipynb
02_topic_modelling_bertopic_pra_mapping.ipynb
03_sentiment_analysis_distilroberta_finetuned.ipynb
04_evasion_detection_deberta_roberta_ranking.ipynb
05_supervisory_summarisation_llm.ipynb
06_ai_agent_financial_supervision.ipynb   (coming soon)

reports/
project_report.pdf

slides/
project_presentation.pdf

data/
sample_jpm_qna.csv
sample_hsbc_qna.csv

agent/
(tools and workflows will be added here)

---

## **5. Notebook Overview**

### **01 · Data Preparation & Extraction**
Parsing raw transcripts, cleaning text, structuring speaker metadata, creating a unified supervisory dataset.

### **02 · Topic Modelling (BERTopic)**
- Finance2 embeddings  
- Topic clustering  
- Mapping themes to PRA categories  
- Evolution of narratives over time  

### **03 · Sentiment Analysis (DistilRoBERTa Fine-tuned)**
- Benchmarking FinBERT vs Cardiff vs DistilRoBERTa  
- Role-based divergence (bankers vs analysts)  
- Quarterly sentiment shifts  

### **04 · Evasion Detection (DeBERTa + RoBERTa Ranking)**
- NLI-based classification  
- Ranking evasive segments  
- PRA-aligned transparency risk clusters  

### **05 · Supervisory Summaries (LLM)**
Structured GPT-4.1 briefings focusing on:

- key risk drivers  
- quarter-over-quarter changes  
- analyst–management discrepancies  
- potential supervisory watch-outs  

### **06 · AI Agent (Coming Soon)**
A multi-tool agent capable of:

- calling topic, sentiment, and evasion modules  
- answering supervisory queries  
- generating risk dashboards  
- assisting analysts interactively  

---

## **6. Selected Insights**

### **Tone Divergence**
Executives consistently demonstrate **more optimistic tone** than analysts — a known supervisory asymmetry.

### **Evasiveness Hotspots**
Detected primarily around:

- capital adequacy  
- liquidity and funding  
- cost efficiency  
- geopolitical exposures  

### **PRA-Aligned Themes**
Topic models map cleanly onto:

- Liquidity  
- Credit risk  
- Governance  
- Conduct  
- Profitability  

### **Forward-Looking Signals**
LLM summaries reveal shifts in:

- deposit stability  
- credit tightening  
- macroeconomic tensions  
- RWA pressures  

---

## **7. Future Work: Supervisory AI Agent**

Planned next stage includes:

- PRA-aligned interactive risk assistant  
- Multi-tool LLM agent  
- Visual risk dashboards  
- Automated quarterly briefings  
- Cross-bank discourse clustering  

This will form the basis of a **RegTech-grade supervisory intelligence system**.

---

## **8. About**

This project combines:

- **Cambridge ML rigor**  
- **Bank of England supervisory framing**  
- **Real JPM & HSBC data**  
- **Modern LLM and NLP methods**  

to demonstrate how AI can augment decision-making in high-trust financial environments.

---
