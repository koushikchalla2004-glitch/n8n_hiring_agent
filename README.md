# n8n Hiring Agent Workflow

A form-based n8n workflow that:
- Collects candidate Name, Email, LinkedIn URL, and Job URL.
- Calls Relevance AI endpoints to fetch profile/job info.
- Uses a Gemini agent to evaluate eligibility.
- Sends a “Selected to apply” or “Not eligible” email via Gmail.

## Import
1. Download `My workflow 3.json`.
2. In n8n: **Workflows → Import from file**.
3. Create credentials:
   - **Google Gemini/PaLM API** using `GEMINI_API_KEY`.
   - **Gmail OAuth2** (`GMAIL_CLIENT_ID`, `GMAIL_CLIENT_SECRET`, `GMAIL_REFRESH_TOKEN`).
4. (Optional) Map Gmail “Send To” to the form’s Email:

