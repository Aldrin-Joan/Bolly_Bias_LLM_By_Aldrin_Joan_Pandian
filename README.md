
# 🎬 Bollywood Bias Buster  
**AI Project | Internship at docu3C Technologies**

---

## 🚀 Overview

This project addresses gender bias in Bollywood movie scripts using large language models (LLMs). It detects, quantifies, and mitigates stereotypical portrayals of women through a multi-phase NLP pipeline.

---

## 📁 File Structure

| File | Purpose |
|------|---------|
| `bolly_data_clean.ipynb` | Phase 1: Script cleaning and preparation |
| `bollyLLM.ipynb` | Phase 2: Bias stereotype classification using LLM (Mistral) |
| `phase3.ipynb` | Phase 3: Bias quantification per movie and stereotype |
| `Phase4A.ipynb` | Phase 4A: Rewriting biased lines with Mistral |
| `Phase4B.ipynb` | Phase 4B: Feedback report generator (CSV + PDF) |

---

## 🧠 Bias Taxonomy

| Stereotype Type | Description |
|-----------------|-------------|
| `occupation_gap` | No mention of professional role or ambition |
| `agency_gap`     | Lack of decision-making, passive portrayal |
| `appearance_focus` | Focus on beauty, clothes, body |
| `relationship_only` | Introduced only as wife/daughter/sister |
| `none`           | Neutral, progressive or unbiased |

---

## ⚙️ Setup

1. **Clone the repo / Upload files to Colab / VS Code**
2. **Install dependencies:**

```bash
pip install -r requirements.txt
```

3. **Ensure GPU is enabled (Colab: Runtime > Change Runtime > GPU)**

---

## 🧪 Phase Summary

| Phase | Goal |
|-------|------|
| **Phase 1** | Load + clean chunked movie script data |
| **Phase 2** | Use LLM (Mistral) to classify stereotypes line-by-line |
| **Phase 3** | Aggregate bias metrics per movie and visualize trends |
| **Phase 4A** | Rewrite biased lines using prompt-based mitigation |
| **Phase 4B** | Generate PDF feedback report with rewrites & severity |

---

## 📁 Outputs & Deliverables
|Phase|	Output File(s)|	Description|
|Phase 1|	cleaned_script_data.csv	|Cleaned and structured dataset with movie lines.|
|Phase 2|	ai_stereotype_annotated_final.csv	|Each line labeled with one of 5 stereotype types.|
|Phase 3|	bias_scores_by_gender.csv, bias_scores_overall.csv, bias_trends_overall.png|	Bias quantification CSVs and trend visualization PNG.|
|Phase 4A|	phase4a_rewrites.csv|	Model-suggested rewrites for biased lines.|
|Phase 4B|	feedback_report.csv, feedback_report.pdf|	Ranked fixes and severity report (tabular + PDF).|

---

## ✅ Evaluation Targets

- ✅ **Detection Accuracy**: ≥ 85% F1 on test set (human annotated)
- ✅ **Rewrite Quality**: ≥ 4/5 human rating for usefulness & clarity

---

## 📌 Notes

- LLM used: **Mistral 7B Instruct** (running locally & via Colab)
- Due to hardware limits, testing and reporting was done on selected chunks.
- Prompt engineering was crucial to obtain clean, single-label predictions and rewrites.
