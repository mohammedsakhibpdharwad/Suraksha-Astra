# Suraksha-Astra: AI-Based Cyber Safety & Content Moderation System

Suraksha-Astra is an end-to-end intelligent cyber safety platform engineered to identify toxic, abusive, and NSFW digital media in real-time using multi-modal AI pipelines. The system combines deep learning architectures with automated enforcement policies to ensure safer online spaces.

---

## Key Features

- **Multi-Modal Threat Detection:** Analyzes textual and visual inputs simultaneously to classify toxic interactions, harassment, and unsafe media.
- **NLP & Computer Vision:** Employs Hugging Face Transformers for contextual text analysis and CNNs (via OpenCV) for visual media scanning and behavioral anomaly detection.
- **Dynamic Risk Engine:** Generates a 0–100 weighted risk score categorizing interactions into `SAFE`, `MONITOR`, `SUSPICIOUS`, and `HIGH RISK`.
- **Automated Enforcement:** Provides sub-second policy actions (`ALLOW`, `LIMIT`, `BLOCK`) through asynchronous endpoints.
- **Moderation Dashboard:** Interactive user interface for auditing incidents, tracking flagged content, and reviewing system enforcement actions.

---

## Tech Stack

- **Backend & APIs:** Python, FastAPI, RESTful APIs, Asynchronous I/O
- **AI / Deep Learning:** Hugging Face Transformers, Computer Vision (CNNs), OpenCV
- **Frontend / Dashboard:** JavaScript, Tailwind CSS, HTML5
- **Tooling & Version Control:** Git, GitHub

---

## Project Architecture

1. **Input Ingestion:** Accepts multi-modal data streams (text snippets, image uploads) via FastAPI endpoints.
2. **Inference Pipeline:**
   - Text streams undergo tokenization and classification through Hugging Face NLP models.
   - Images and frames are processed with OpenCV and evaluated via CNN classifiers.
3. **Risk Scoring Engine:** Normalizes confidence metrics into a unified 0–100 threat index.
4. **Action Dispatcher:** Automatically triggers `ALLOW`, `LIMIT`, or `BLOCK` actions based on configurable safety thresholds.

---

## Getting Started

### Prerequisites
- Python 3.10+
- Git

### Installation

1. Clone the repository:
   ```bash
   git clone [https://github.com/](https://github.com/)<your-username>/suraksha-astra.git
   cd suraksha-astra
