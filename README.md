# Al-Powered-Cold--Outreach-Follow-Up-Automation
Designed a scalable email automation platform using n8n, Google Gemini, Gmail API, and Google Sheets. Built end-to-end workflows for lead ingestion, LLM-based generation, Gmail delivery, and reliable state persistence. Implemented conditional logic, scheduling, and duplicate-safe processing, demonstrating backend orchestration and API integration.
Designed a scalable email automation platform using n8n, Google Gemini, Gmail API, and Google Sheets. Built end-to-end workflows for lead ingestion, LLM-based generation, Gmail delivery, and reliable state persistence. Implemented conditional logic, scheduling, and duplicate-safe processing, demonstrating backend orchestration and API integration. Lead Ingestion & Data Normalization • Reads lead data (company, role, email, job link) • Normalizes fields for downstream consistency • Assigns deterministic row identifiers for updates

Concepts: ETL, data validation, idempotency

⸻

2️⃣ AI-Powered Email Generation • Uses Google Gemini (LLM) to generate: • Context-aware subject lines • Personalized email bodies • Prompt engineered for professional tone and relevance

Concepts: Prompt engineering, LLM integration, NLP

⸻

3️⃣ Email Sending & Thread Management • Sends emails using Gmail API • Captures message ID and thread ID • Ensures follow-ups remain in the same email thread

Concepts: API integration, transactional email systems

⸻

4️⃣ State Tracking & Persistence • Updates Google Sheets with: • Email sent status • Timestamps • Generated email content • Gmail message metadata • Uses row-level matching for reliable updates

Concepts: State management, idempotent updates

⸻

5️⃣ Automated Follow-Up System • Scheduled workflow runs daily • Sends follow-ups: • Follow-up #1 after 3 days • Follow-up #2 after 7 days • Prevents duplicate follow-ups using conditional checks

Concepts: Event-driven systems, cron scheduling

⸻

🧩 n8n Nodes Used • Google Sheets (Read / Update Row) • Set / Edit Fields • IF (Conditional logic) • Google Gemini – Message a Model • Gmail – Send Message • Date & Time • Schedule Trigger

⸻

🛠 Tech Stack • JavaScript • n8n • Google Gemini (LLM) • Gmail API • Google Sheets API • Workflow Automation • ETL Pipelines

⸻

✅ Key Features • Scalable personalized outreach • AI-generated content • Reliable state persistence • Thread-safe follow-ups • Duplicate send prevention • Modular and reusable workflows

⸻

📈 Real-World Use Cases • Recruiting outreach • Sales development automation • Customer engagement workflows • AI-assisted communication platforms

⸻

🔐 Notes on Security • Credentials managed securely via n8n credentials • Sensitive data (emails, tokens) not stored in code • Supports easy credential rotation

⸻

📌 Future Enhancements • Reply detection and auto-stop follow-ups • Email rate limiting & warm-up logic • Dashboard for analytics • CRM integration (HubSpot / Salesforce)
