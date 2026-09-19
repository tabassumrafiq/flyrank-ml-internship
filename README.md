# FlyRank ML Internship — Starter Repo

**Applied Search Intelligence: Google Search Ranking & Discoverability**

This is the starting point for the FlyRank ML Internship. You **clone it into your own public
repo** (one click — *Use this template*), build everything there, and submit that repo URL on
each assignment in your portal — it's your workspace, your submission, and your portfolio all
at once. The rhythm is simple: do the work, commit it, submit on the card. Done.

Everything here runs on a small **anonymized** slice of real FlyRank search data. No credentials,
no private client data, no setup headaches.

> **New here?** Two reads: **[SETUP.md](SETUP.md)** (GitHub, Colab, and data access — ten
> minutes, with every silent pitfall flagged), then **[GUIDE.md](GUIDE.md)** (every file
> explained, what to edit vs. leave alone, and where your own work goes — five minutes).

---

## Quickstart — first win in 2 minutes

The fastest path is Google Colab (one click, zero install). Open Notebook 1 and run all cells:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tabassumrafiq/flyrank-ml-internship/blob/main/notebooks/01_first_look_and_discovery.ipynb)
 **Week 1 — Run it, then discover a real truth yourself**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tabassumrafiq/flyrank-ml-internship/blob/main/notebooks/02_your_first_readable_model.ipynb)
 **Week 2 — The model is just a rule you can read**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tabassumrafiq/flyrank-ml-internship/blob/main/notebooks/03_working_with_the_full_release.ipynb)
 **Weeks 3+ — The full release (~79M rows) via DuckDB, no download needed** — hosted at
 [`FlyRank/internship-warehouse`](https://huggingface.co/datasets/FlyRank/internship-warehouse) (gated: request access + accept the data-use terms, approval is instant)

---

## Your assignment notebooks — open, fill, save, done

Every assignment is one pre-named skeleton notebook in `work/notebooks/`. Click its badge,
fill the sections in order, then **File → Save a copy in GitHub → OK** — the dialog is
already pre-filled with your repo and the right path.

> **The badges know whose repo they're in.** About 30 seconds after you create your copy, an
> automatic commit ("Point Colab badges at this copy") rewires every badge in it to open
> **your** notebooks — with your saved work — instead of the shared read-only ones. Reading
> this on the shared starter page? The badges below open blank previews; make your copy
> first ([SETUP.md](SETUP.md), Moment 1).

| Week | Card | Notebook | Open |
|---|---|---|---|
| 1 | ML-02 | `w01_research_question` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tabassumrafiq/flyrank-ml-internship/blob/main/work/notebooks/w01_research_question.ipynb) |
| 2 | ML-03 | `w02_ml_task_framing` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tabassumrafiq/flyrank-ml-internship/blob/main/work/notebooks/w02_ml_task_framing.ipynb) |
| 3 | ML-04 | `w03_data_contract` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tabassumrafiq/flyrank-ml-internship/blob/main/work/notebooks/w03_data_contract.ipynb) |
| 3 | ML-05 | `w03_feature_leakage_check` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tabassumrafiq/flyrank-ml-internship/blob/main/work/notebooks/w03_feature_leakage_check.ipynb) |
| 4 | ML-06 | `w04_signal_audit` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tabassumrafiq/flyrank-ml-internship/blob/main/work/notebooks/w04_signal_audit.ipynb) |
| 4 | ML-07 | `w04_baseline_score` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tabassumrafiq/flyrank-ml-internship/blob/main/work/notebooks/w04_baseline_score.ipynb) |
| 5 | ML-08 | `w05_model` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tabassumrafiq/flyrank-ml-internship/blob/main/work/notebooks/w05_model.ipynb) |
| 6 | ML-09 | `w06_validation_audit` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tabassumrafiq/flyrank-ml-internship/blob/main/work/notebooks/w06_validation_audit.ipynb) |
| 7 | ML-10 | `w07_action_playbook` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tabassumrafiq/flyrank-ml-internship/blob/main/work/notebooks/w07_action_playbook.ipynb) |
| 8 | ML-11 | `capstone` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tabassumrafiq/flyrank-ml-internship/blob/main/work/notebooks/capstone.ipynb) |

Badges not opening *your* copy? Colab's built-in opener always works: **File → Open notebook
→ GitHub tab** → paste `github.com/you/your-repo` → pick the notebook.

### Prefer local?

```bash
git clone <this-repo-url>
cd flyrank-ml-internship-starter
pip install -r requirements.txt          # or: uv pip install -r requirements.txt
python scripts/run_all.py
```

That runs the whole pipeline on the bundled sample and writes results to `outputs/`.

---

## What you get

| Path | What it is |
|---|---|
| `notebooks/` | Week 1–2 **first-win notebooks** (Colab-ready). Start here. |
| `scripts/01–05` + `run_all.py` | The runnable reference pipeline: prepare → baseline → train → evaluate → PDF. |
| `data/raw/content_refresh_anonymized.csv` | The anonymized starter dataset (~30k pages). |
| `outputs/` | Example outputs so you can see the **target shape** (`model_report.md`, `refresh_queue_sample.csv`, `charts/`). |
| `work/` | **Your space.** Lane experiments and your capstone live here — see `work/README.md`. |
| `docs/` | The core docs + the data dictionary (see below). |

### Read these (in `docs/`)

1. **`ml-core-foundation-framework.md`** — the first-principles map of ML as a whole system. The backbone of the live sessions.
2. **`ml-intern-dataset-and-lane-guide.md`** — how to use the data safely, the capstone workflow, and the analysis "lanes" you can pick from.
3. **`intern-free-tooling-guide.md`** — the zero-budget tool stack (Python, Colab, free AI assistants). You never need to pay for anything.
4. **`data-dictionary.md`** — all 44 columns: meaning, scale, and gotchas. Keep it open while you work.

---

## The pipeline (what `run_all.py` does)

```text
01_prepare_features.py   clean + build the feature vector, define the label
02_baseline_score.py     a transparent hand-rule "fix this first" score
03_train_model.py        logistic regression, decision tree, random forest (client-holdout split)
04_evaluate_and_export.py  ranked queue + charts + Markdown report
05_build_pdf_report.py   a shareable PDF summary
```

On the bundled sample, the learned model clearly beats the hand-written rule at picking the right
pages to review first (**Precision@50 ≈ 0.24 → 0.74**; the model number can land 0.68–0.74
depending on library versions — the ~3x lift is the point). The notebooks compute these numbers
live, so they always reflect the current data and environment.

**Teaching point:** the model is the capstone, but the *workflow* is the lesson —
`problem framing → data cleaning → baseline → first model → evaluation → explainable recommendation`.

---

## Data safety (read `DATA_USE.md`)

- Only the small **anonymized** CSV ships here — no client names, domains, URLs, titles, or keywords.
- **Never** add raw private client data to this repo or your fork. Need more data? Request an approved
  release from your mentor — never export it yourself.
- Don't paste client data into third-party AI tools.
- Frame every result as **observed / measured / directional / decision-support** — never
  "I predicted Google's algorithm."

The `.gitignore` blocks datasets by default, and CI fails any commit that includes a dataset.

---

## Assignments & schedule

Weekly assignments, live events, and the capstone live on **your portal board** (your
enrollment email has your access link). This repo is the shared technical foundation they all
build on — and the `skills/` folder here is the instruction library for your AI assistant
(start at [skills/README.md](skills/README.md)).

**First time with GitHub?** You need exactly four things (full walkthrough: [SETUP.md](SETUP.md)):
1. A free account at github.com.
2. Your own copy of this repo: **Use this template → Create a new repository** → public.
   (One click — brings the notebooks, `work/`, and the CI leak-guard with it.)
3. In Colab: *File → Save a copy in GitHub* — opened from your copy's badges, the dialog is
   already pre-filled with your repo and path, so it's just OK (Colab handles auth).
4. That's your submission repo — share its **github.com/you/your-repo** URL with Assignment 1
   (never a colab.research.google.com or drive.google.com link).

---

*Track leads: Mirza Ašćerić (ML) · Hole (data engineering). Code under MIT (see `LICENSE`); data under `DATA_USE.md`.*


FlyRank ML Internship — Starter Repo

Applied Search Intelligence: Google Search Ranking & Discoverability

This is the starting point for the FlyRank ML Internship. You clone it into your own public repo, build everything there, and submit that repo URL on each assignment in your portal — it's your workspace, your submission, and your portfolio all at once.

Everything here runs on a small anonymized slice of real FlyRank search data. No credentials, no private client data, no setup headaches.

Quickstart

The fastest path is Google Colab.

Local Setup

git clone https://github.com/tabassumrafiq/flyrank-ml-internship.git
cd flyrank-ml-internship
pip install -r requirements.txt
python scripts/run_all.py

The pipeline runs on the bundled anonymized sample and writes results to outputs/.

Assignment Notebooks

Every assignment is available inside work/notebooks/.

1. Week 1 — ML-02 — w01_research_question
2. Week 2 — ML-03 — w02_ml_task_framing
3. Week 3 — ML-04 — w03_data_contract
4. Week 3 — ML-05 — w03_feature_leakage_check
5. Week 4 — ML-06 — w04_signal_audit
6. Week 4 — ML-07 — w04_baseline_score
7. Week 5 — ML-08 — w05_model
8. Week 6 — ML-09 — w06_validation_audit
9. Week 7 — ML-10 — w07_action_playbook
10. Week 8 — ML-11 — capstone

What You Get

• notebooks/ — Week 1–2 first-win notebooks
• scripts/ — Runnable reference pipeline
• data/raw/ — Anonymized starter dataset
• outputs/ — Example outputs
• work/ — My assignment and capstone work
• docs/ — Project documentation and data dictionary

The Pipeline

01_prepare_features.py → 02_baseline_score.py → 03_train_model.py → 04_evaluate_and_export.py → 05_build_pdf_report.py

Workflow:
Problem Framing → Data Cleaning → Feature Engineering → Baseline → Machine Learning Model → Evaluation → Actionable Recommendation

Data Safety

• Only anonymized data is used in this repository.
• No private client data should be added.
• No credentials or sensitive information should be committed.
• Results should be treated as observed, measured, directional, and decision-support evidence.
• The project does not claim to predict Google's ranking algorithm.

Bibi Tabassum — ML Capstone

What the Project Does

This project focuses on identifying website content that may be declining in search performance and prioritizing pages for review or refresh.

The system uses machine learning and content-performance signals to help SEO teams decide which pages should be reviewed first.

It is designed as a decision-support tool, not as a system that predicts or explains Google's ranking algorithm.

Who It Is For

The project is intended for:
• SEO teams
• Content teams
• Website managers
• Digital marketing teams

It can help teams identify content that may need further investigation, review, or refresh.

Problem Statement

Websites can contain pages whose search performance is declining over time. Manually reviewing a large number of pages can be difficult and time-consuming.

This project explores a machine-learning-based approach for identifying potentially declining content and prioritizing pages for review.

Dataset

The project uses the anonymized content_refresh_anonymized.csv dataset provided through the internship repository.

The dataset contains approximately 30,000 rows and multiple content and search-performance fields.

No private client names, domains, URLs, titles, or keywords are used.

Target

The target label is derived from the content trend direction:

is_declining_label = trend_direction == "down"

The objective is to identify content associated with a declining trend and prioritize it for further review.

Features Used

The project uses content and search-performance signals including:
• avg_position
• ctr
• engagement_rate
• scroll_rate
• word_count

These features provide information about search visibility, user engagement, and content characteristics.

Architecture

Anonymized Content Data
        ↓
Data Preparation
        ↓
Feature Engineering
        ↓
Target Definition
        ↓
Baseline Scoring
        ↓
Machine Learning Model
        ↓
Validation & Evaluation
        ↓
Action / Review Queue
        ↓
Content Review or Refresh

Model Evaluation

The project evaluates the machine-learning workflow using classification metrics and validation strategies.

Two evaluation approaches are considered:
1. Random split
2. Client-grouped split

Client-grouped validation is important because pages belonging to the same client should not be mixed between training and testing data when evaluating generalization.


### v2 Evaluation Results

The final v2 evaluation compared a Random Forest model using a random split and a client-grouped split.

| Metric | Random Split | Client-Grouped Split |
|---|---:|---:|
| Accuracy | 0.6352 | 0.5398 |
| Precision | 0.6121 | 0.5283 |
| Recall | 0.8924 | 0.9270 |
| F1 | 0.7261 | 0.6730 |

The client-grouped split had no client overlap between training and test data and is treated as the more conservative estimate of generalization to unseen clients.

The grouped validation result shows a measurable directional signal, but the lower grouped performance indicates that the model should be treated as decision-support rather than production-grade prediction.

The baseline used 28,795 valid content items and prioritized the top 10% using an equal-weight combination of percentile-ranked 90-day impressions and average search position.

Neither the baseline nor the model proves that an individual content item will decline or that a particular refresh action will improve future performance.

limitation

• The dataset is anonymized and represents a limited view of real-world search performance.
• The available features do not capture every factor that may influence search performance.
• Model performance can vary depending on the data and environment.
• The model should not be interpreted as predicting Google's ranking algorithm.
• Machine-learning results require human interpretation.
• A high-priority page still requires human review before making content or SEO changes.
• Results should be treated as directional and decision-support evidence rather than universal conclusions.

Key Design Decision

A key design decision was to use client-grouped validation in addition to a random split.

The grouped approach helps evaluate whether the model can generalize to clients that were not represented in the training data and reduces the risk of overly optimistic evaluation caused by client overlap.

What Was Built With AI

AI assistance was used during the project for:
• Understanding assignment requirements
• Brainstorming and refining implementation approaches
• Debugging and reviewing code
• Improving documentation
• Reviewing explanations
• Helping structure the project workflow

The final implementation, analysis, evaluation, outputs, and project decisions were reviewed and completed as part of the internship work.

How to Use the Capstone

1. Open the capstone notebook: work/notebooks/capstone.ipynb
2. Load the anonymized dataset.
3. Prepare the required features.
4. Define the declining-content target.
5. Run the baseline.
6. Train the machine-learning model.
7. Run the evaluation.
8. Review the generated outputs.
9. Use the resulting scores as a starting point for content review and refresh decisions.

Project Repository

GitHub Repository:
https://github.com/tabassumrafiq/flyrank-ml-internship

Internship Learning Outcome

This capstone demonstrates an end-to-end machine-learning workflow:

Research Question → Problem Framing → Data Contract → Feature & Leakage Checks → Signal Analysis → Baseline → Model → Validation → Action Playbook → Capstone

The main focus is not only the final model, but also the complete workflow from problem definition to evaluation and actionable decision support.

Author

Bibi Tabassum
Artificial Intelligence Student
Abdul Wali Khan University Mardan (AWKUM)

GitHub: https://github.com/tabassumrafiq
LinkedIn: https://www.linkedin.com/in/bibi-tabassum-2027402a/
