# PromptGuard System (3-Layer Adversarial Guardrail)

An enterprise-grade, low-latency prompt injection defense gatekeeper designed to secure LLM applications. This repository implements an optimized early-exit pipeline using structural heuristics, a machine learning classifier, and a high-precision generative judge framework.

## 📁 Repository Directory Structure

- `data/` - Holds local data splits (`raw/` data tracks and `processed/` matrix rows). Managed completely out of version control index (Explicitly load for  hugging face using "Necent/llm-jailbreak-prompt-injection-dataset").
- `notebooks/` - Exploratory analysis, feature selection workflows, and model training matrices.
- `src/` - Production codebase engine.
  - `src/api/` - FastAPI model serving controllers and deployment endpoints.
  - `src/pipeline/` - Data vectorization, token validation routines, and inference processors.
- `tests/` - Automated unit test routines managed through `pytest`.

## ⚙️ Initial Developer Workspace Setup

Follow these precise steps to get the environment running locally on your workstation:

### 1. Reconstruct the Virtual Environment
```bash
# Initialize a local virtual environment container
python3 -m venv venv

# Activate the local execution shell
source venv/bin/activate

# Install the exact software matrix packages
pip install -r requirements.txt