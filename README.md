# Conversational SMS AI Agent — GoHighLevel + n8n (Concept Demo)

Interactive concept demo for a **conversational SMS agent** built on a GoHighLevel
inbound-SMS webhook, an n8n orchestration workflow, and an LLM.

- **Live demo:** https://awaissattar763-ctrl.github.io/sms-ai-agent-demo/
- `index.html` — phone-style SMS chat simulation (scripted replies that mirror the
  production agent's behavior: qualification, pricing guardrails, booking, human handoff)
- `workflow.json` — import-ready n8n blueprint:
  `Webhook → GHL contact lookup → Switch(intent) → OpenAI → GHL SMS reply → contact update`,
  with a human-escalation branch and error-handler reference

**Honest labeling:** every reply in the chat is a scripted simulation of the
production behavior. No live GHL or n8n backend is connected. This demo was built
as a targeted proposal asset — it shows approach, not a client deployment.
