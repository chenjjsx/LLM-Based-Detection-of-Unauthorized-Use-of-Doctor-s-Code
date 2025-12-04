Structured Prompts for LLM-Based Detection of Unauthorized Use of Doctor’s Code

This repository provides the structured prompt templates used for large language model (LLM)–based semantic plausibility assessment in the task of detecting Unauthorized Use of Doctor’s Code in health-insurance claim records.

⚠️ No real or de-identified medical data is included in this repository.
⚠️ Only prompt templates and input-format examples are released, to support reproducibility while complying with strict data-privacy regulations.

⸻

🔍 Purpose of This Repository

The prompts included here are designed to:
	•	guide an LLM to distinguish reasonable medical behaviors from unauthorized use in rule-flagged claim record pairs,
	•	enforce structured, deterministic outputs, and
	•	reduce false positives in health-insurance audit workflows.

These prompts were used in our study to evaluate LLM reasoning behavior under different prompting strategies.

⸻

📂 Contents

1. Structured Prompts (S-Prompt)

Templates with explicit reasoning rules and allowed legitimate scenarios:
	•	Cross-Institution Scenario (S-Prompt)
	•	Cross-Department Scenario (S-Prompt)

2. Weakly-Structured Prompts (W-Prompt)

Templates providing partial contextual rules without strict output constraints:
	•	Cross-Institution Scenario (W-Prompt)
	•	Cross-Department Scenario (W-Prompt)

3. Zero-Prompt Baselines

Minimal task instructions with no prompting structure:
	•	Cross-Institution Zero-Prompt
	•	Cross-Department Zero-Prompt

⸻

🧩 How to Use
	1.	Insert a record pair into the example input template.
	2.	Select one of the prompts (S-Prompt, W-Prompt, or Zero-Prompt).
	3.	Call your preferred LLM API (local or online), providing the chosen prompt as the system prompt.
	4.	Parse the model output:
	•	"Reasonable, <scenario>"
	•	"Unauthorized"

⸻

⚠️ Notes on Data Privacy

Due to the sensitive nature of medical-insurance data, no sample records, no real fields, and no claim data can be released.
Only prompt templates are included now.

⸻
