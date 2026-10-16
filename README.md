# Heng (Kyo) Xu · Graduate AI Engineer, Sydney

I build Python services around language models: agent workflows, retrieval, model evaluation and serving, and the guardrails that keep AI coding agents inside the rules they were given.

## Selected work

### EntryPlug: governance for AI coding agents
**Public** · [github.com/Blacksun10282022/entryplug](https://github.com/Blacksun10282022/entryplug)

A CLI and MCP server that lets an AI coding agent (Claude Code or Codex) work from one person's written rules and notes, while keeping it from changing them or sending anything out in their name unasked.

- Protected files are enforced in code, not in the prompt: a Git pre-commit hook plus Claude Code deny rules; changes go through an owner-approved request.
- A PreToolUse hook refuses the common outbound write commands (`git push`, HTTP POST, mail, publish tools), verified live in both Claude Code and Codex sessions.
- Read-only MCP search over the notes (SQLite FTS5, Chinese and English): recall@10 0.98 on a public 50-case gold set; 134 unit tests.

### AI-Powered PII Detection and Redaction Service: USYD capstone (High Distinction)
**Public portfolio edition** · [github.com/Blacksun10282022/AI-Powered-PII-Detection-and-Redaction-Service](https://github.com/Blacksun10282022/AI-Powered-PII-Detection-and-Redaction-Service)

An 8-person, client-delivered project; I led backend and deployment.

- FastAPI service for text, DOCX, PDF and images (OCR), with versioned masking policies and structured entity spans.
- Fine-tuned student model: F1 0.9775 against the teacher's 0.9505 on a 14,000-row holdout, compared through vLLM-served inference.
- Docker and GitHub Actions CI; client deployment validated on an on-prem DGX Spark.

### Luna: local desktop AI companion
[github.com/Blacksun10282022/Local-desktop-AI-companion-Luna](https://github.com/Blacksun10282022/Local-desktop-AI-companion-Luna)

Electron + FastAPI, llama.cpp-served Qwen2 models, local/cloud fallback, startup orchestration and health checks.

## Stack

Python · SQL · FastAPI · Pydantic · pytest · PyTorch · RAG · MCP · vLLM · PostgreSQL / pgvector · DuckDB · Docker · AWS · Terraform · GitHub Actions · Claude Code · Codex

## Contact

[LinkedIn](https://linkedin.com/in/heng-xu-557892320)
