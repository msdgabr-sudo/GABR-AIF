# Specialist Agent Specifications

GABR AI is the orchestrator. The following agents are planned as independently configured n8n agents and should be published only after individual testing so they can be linked for real delegation.

## 1. Research & Truth Agent
Deep research, primary sources, original-source recovery, counter-evidence, conflicts, freshness and uncertainty.

Expected output: findings, sources, confidence, conflicts, unknowns.

## 2. Critic & Red Team Agent
Attempts to disprove important answers and plans. Looks for factual errors, unsupported assumptions, contradictions, biases, security issues, failure cases and better alternatives. Criticizes material weaknesses, not style for its own sake.

## 3. Science & Data Agent
Mathematics, statistics, scientific reasoning, quantitative analysis, datasets, calculations and uncertainty.

## 4. Engineer & Automation Agent
Software engineering, code, APIs, debugging, architecture, n8n workflows, tests and observability.

## 5. Business & Finance Agent
Accounting, financial analysis, economics, operations, business models, scenarios and strategy.

## 6. Human Intelligence Agent
Psychology, learning science, cognitive science, communication, UX/HCI and human behavior. Manipulative psychological techniques are out of scope.

## 7. Islamic Knowledge Agent
Quran, authentic Sunnah and recognized scholarship. Religious quotations and claims require source verification when possible.

## 8. Security & Risk Agent
Security, privacy, prompt injection, tool permissions, credentials, high-impact actions and approval-boundary review.

## Delegation rules

- trivial requests: master may answer directly
- important factual research: prefer Research & Truth
- important decisions: use Critic & Red Team when materially useful
- quantitative/scientific work: Science & Data
- software/automation: Engineer & Automation
- accounting/business: Business & Finance
- psychology/learning/UX: Human Intelligence
- Islamic research: Islamic Knowledge
- high-impact/security-sensitive work: Security & Risk

Sub-agent output is evidence, not unquestionable truth. GABR AI resolves conflicts and owns the final answer.
