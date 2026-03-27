Markdown
# 🚀 PTTPLC Gemini Enterprise Workshop: Agent Creation

<img width="512" height="512" alt="qrcode" src="https://github.com/user-attachments/assets/4da2b85d-25e9-4f96-a2cb-ac5cf2cd68b9" />

Link to download the file https://ptt.listedcompany.com/misc/one-report/ptt-one-report-2025-en.pdf<br>

---

## 🛠️ Step 1: Initial Setup

Follow the activities below to initialize your custom AI Auditor.

| Activity | Action / Input |
| :--- | :--- |
| **Start** | Click on **Create Agent** |
| **Interface** | Click on **Proceed to Builder** |
| **Type** | Click on **Agent** |
| **Name** | `Annual Report Test Agent` |
| **Description** | `Annual Report Test Agent` |

---

## ⚙️ Step 2: Configuration & Logic

### 📜 System Instructions
**Activity: Add Instructions**

> [!IMPORTANT]
> Copy and paste the text below into the **Instructions** field to define the agent's persona and strict source constraints.

```text
You are an expert auditor. Your only source of truth is the attached PTT One Report. 
You must identify inconsistencies, hidden risks, and compliance gaps within this specific text. 
Always provide page references.
```

🧠 Model & Knowledge Base<br>
Model Selection: Gemini 3.1 Pro<br>
Knowledge Source: Download PTT One Report 2025<br>
Activity: Upload the file ptt-one-report-2025-en.pdf into the Knowledge section.<br>

```text
💾 Step 3: Deployment
[x] Activity: Click on Save Agent
[x] Activity: Click on Chat with Agent
```
🧪 Specialized Testing Rounds
Use these predefined prompts to audit the document through the chat interface.
🔍 Round 1: Greenwashing & Consistency Check
Prompt:
Compare the CEO’s statement regarding 'Green Energy Investment targets' in the opening pages against the actual 'Capital Expenditure' breakdown in the Financial Statements section. Are the numbers and timelines consistent? Identify any vague language that could be flagged as 'Greenwashing' risk.
```text
🛡️ Round 2: Fraud & Control Gap Simulation (The "What-If" Test)
Prompt:
Based on the 'Internal Control' and 'Risk Management' sections described in this report, walk me through a hypothetical scenario where a vendor could bypass the 'Procurement Oversight' process without being detected. What specific control is the weakest link according to the text?
```
⚖️ Round 3: Regulatory "Stress Test" (SEC/ESG Alignment)
Prompt:
Act as an SEC Thailand Regulator. Review the 'Corporate Governance' chapter. List 5 critical questions you would ask PTT's Board of Directors based on the gaps in this disclosure. Focus on 'Conflict of Interest' and 'Board Diversity'.
[!TIP]
Workshop Note: If the agent provides an answer without a specific location, prompt it with: "Which page of the PTT One Report does this information come from?"
[!CAUTION]
Ensure the uploaded PDF is fully indexed before running the Specialized Testing Rounds to ensure maximum accuracy.
