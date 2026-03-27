Markdown
# 🚀 PTTPLC Gemini Enterprise Workshop: Agent Creation

<img width="512" height="512" alt="qrcode" src="https://github.com/user-attachments/assets/4da2b85d-25e9-4f96-a2cb-ac5cf2cd68b9" />

Link to download the file https://ptt.listedcompany.com/misc/one-report/20260324-ptt-financial-report-2025-en.pdf<br>
Link to download the file https://ptt.listedcompany.com/misc/one-report/20260324-ptt-supplementary-2025-en.pdf<br>

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
Knowledge Source: Download PTT Reports<br>
Activity: Upload the files into the Knowledge section.<br>


💾 Step 3: Deployment<br>
[x] Activity: Click on Create Agent<br>
[x] Activity: Click on Chat with Agent<br>

🧪 Specialized Testing Rounds<br>
Use these predefined prompts to audit the document through the chat interface.<br>
🔍 Round 1: Strategy vs. Execution (The "Reality Check")<br>
Prompt:<br>
```text
Review the 'Electric Vehicle Business (EV)' section. Management states they are reviewing the EV business model to align with the competitive environment. However, this involves the divestment of Neo Mobility Asia Co., Ltd. (NMA) and Contemporary Amperex Technology Co., Ltd. (CATL), as well as the dissolution of Swap & Go Co., Ltd.. Cross-reference these operational retreats with the 'New Business and Sustainability' financial statements. Are these capital reallocations and strategic shifts clearly justified by the financial data, and do they indicate a risk of unrecorded sunk costs?
```

🛡️ Round 2: Vendor/Contractor Risk & Control Gap Simulation<br>
Prompt:<br>
```text
Examine the 'Clean Fuel Project (CFP)' updates under Thai Oil Public Company Limited (TOP) alongside the related arbitration proceedings. The report states the Main Contractor failed to pay subcontractors, leading to work stoppages, an EPC contract termination, and a massive project cost increase of approximately USD 1,776 million. From an internal audit perspective, what specific procurement and vendor due diligence controls failed here? Furthermore, what financial exposure remains tied up in TOP's 'Construction in Progress' assets?
```
⚖️ Round 3: Financial "Stress Test" (Impairment & Liquidation Analysis)<br>
Prompt:<br>
```text
Act as a Lead Financial Auditor. Identify all subsidiaries currently undergoing judicial reorganization, dissolution, or liquidation, such as Vencorex France S.A.S.U., PTT Energy Solutions (PTTES), and PTT Energy Resources (PTTER). Specifically, analyze the Baht 1,842 million difference recognized from the de-consolidation of the Vencorex subsidiaries. Based on the disclosures, were these impairment losses adequately provisioned for in previous periods, and are there other subsidiaries within the PTTGC or PTTGM groups showing similar early warning signs of asset impairment?.
```
[!TIP]<br>
Workshop Note: If the agent provides an answer without a specific location, prompt it with: "Which page of the PTT One Report does this information come from?"<br>
[!CAUTION]<br>
Ensure the uploaded PDFs (both the Operational Supplementary and the Financial Report) are fully indexed before running the Specialized Testing Rounds. Financial audits require the agent to seamlessly cross-reference narrative claims in Part 1 with the hard data and auditor notes in Part 2.<br>
