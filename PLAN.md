# Project Roadmap (High Level)

This project is a learning-focused system built to analyze database schemas using AI.
The goal is to understand structure, metadata, and reasoning — not to rush into tooling.

---

## Step 1: Python Environment Setup
- Decide and lock Python version (Python 3.11)
- Initialize Pipenv environment
- Verify `python` and `pip` inside the virtual environment
- Commit `Pipfile` and `Pipfile.lock`

**Outcome:** Reproducible, isolated development environment.

---

## Step 2: Project Skeleton
- Define basic folder structure
- Add entry point (`main.py` or `cli.py`)
- Add `.gitignore`
- Add initial README placeholder

**Outcome:** Clean, organized project layout before logic begins.

---

## Step 3: Dummy Database Design
- Choose database type (SQLite)
- Design schema intentionally (tables, columns, relationships)
- Create schema initialization script
- Seed database with fake/sample data

**Outcome:** Safe, predictable dataset for analysis.

---

## Step 4: Core Database Introspection (No AI)
- Connect to database
- Read schema metadata
- Extract tables, columns, data types, constraints
- Output structured metadata (e.g. JSON)

**Outcome:** Clear understanding of what exists in the database.

---

## Step 5: Define AI Contract
- Decide what metadata is sent to the AI
- Decide expected output format (strict JSON)
- Define scope (per-table vs whole-database analysis)
- Validate outputs before use

**Outcome:** Stable, testable interface between core logic and AI.

---

## Step 6: AI Integration (Ollama)
- Integrate local LLM via Ollama
- Implement prompt handling
- Handle token limits and failures
- Ensure deterministic, debuggable behavior

**Outcome:** AI-assisted reasoning layered on top of solid fundamentals.

---

## Step 7: Persist and Review Results
- Store AI responses (raw and parsed)
- Version analysis runs
- Enable re-runs and comparisons

**Outcome:** Repeatable, inspectable analysis instead of one-off output.

---

## Guiding Principles
- Environment first, logic second, AI last
- Prefer clarity over cleverness
- AI assists reasoning — it does not replace understanding
- Every step should be explainable to a beginner
