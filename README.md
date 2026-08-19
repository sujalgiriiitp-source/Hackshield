# AgentBreak

> **Break your AI agent before it breaks the real world.**

AgentBreak is a hackathon prototype for **OOSC 4.0 – Problem Statement 4: AI Agent Evaluation and Reliability Engine**.

It demonstrates an automated red-team evaluation workflow for tool-using AI agents:

`Agent Profile → Adversarial Scenario Generation → Sandboxed Simulation → Failure Classification → Reliability Score → Evidence Report`

## Prototype capabilities
- Adversarial scenario generation across hallucination, prompt injection, tool misuse, goal drift, destructive action and loop-risk categories.
- Safe browser-side sandbox simulation using mocked tools.
- Trace-level evidence for failed tests.
- Weighted reliability score and severity breakdown.
- JSON report export.
- No API key required for the demo.

## Run locally

```bash
python3 -m http.server 8000
```

Open `http://localhost:8000`.

## Demo flow
1. Choose an agent profile.
2. Generate an adversarial suite.
3. Run the reliability evaluation.
4. Inspect the score and failure cards.
5. Open a failed test to inspect its trace.
6. Export the JSON report.

## OOSC PS4 alignment
The prototype demonstrates the PS4 concepts of scenario generation, sandbox replay, failure-mode classification, destructive-action guardrail testing, and reliability scorecards/regression-oriented reports.

## Roadmap
- Real execution adapters for popular agent frameworks.
- Container-isolated workers.
- LLM-as-judge calibration.
- GitHub Actions continuous evaluation.
- Version-to-version regression comparison.

## Team
**Hackshield2.0** — OOSC 4.0 Hackathon
