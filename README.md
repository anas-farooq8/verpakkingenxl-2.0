## VerpakkingenXL Lead Processing 2.0 (Zendesk → Pipedrive)

> AI-assisted B2B lead qualification for Zendesk users, powered by n8n, Google Gemini and Pipedrive.

![n8n](https://img.shields.io/badge/n8n-Workflow-EA4B71?logo=n8n)
![Google Gemini](https://img.shields.io/badge/Google_Gemini-AI-4285F4?logo=google)
![Pipedrive](https://img.shields.io/badge/Pipedrive-CRM-0BB04B.svg?logo=data:image/png;base64,AAABAAUAEBAAAAEAIABoBAAAVgAAABAQAAABACAAaAQAAL4EAAAQEAAAAQAgAGgEAAAmCQAAEBAAAAEAIABoBAAAjg0AABAQAAABACAAaAQAAPYRAAAoAAAAEAAAACAAAAABACAAAAAAAAAEAAATCwAAEwsAAAAAAAAAAAAAAAAAAACAAAIAAAAAAAAAADt7CThAexybPXkV2zd3Avs3dwH7NncB3Dh4AJs3dgA4AAAAAAAAAAAAgAACAAAAAACAAAIAAAAAQIAABDd3A5g1dwD/FHQA/xZwAP82dwD/N3cC/zh5AP86fgH/OHkB/zh2AJczZgAFAAAAAACAAAIAAAAAM2YABTh3BLo4fwD/RH4c/oGkbPt8oWf+PHkQ/zV2AP83dwL+N3cB+zd2Af47gAH/N3cBukCAAAQAAAAAAAAAADh2Apc/gg//I3EA+WWSS/78/vr/8/fw/06BNf85eAz/Q3sk/zt5EP83dwH+N3cB+TuAAf83dwKYAAAAADd2ADg4eQH/OngP/iNwAP5mkUz//v79//b49P9EfCj/AGEA/wBlAP8kcAD/PXkZ/zd3AP43dgH+OHgB/zd2ADg4dwCcOn4B/zt4D/sjcAD/ZZFM//3+/f/z9fH/Z5NM/6e7nv+rvqL/aJNN/wBsAP87eBP/N3cA+zp+Af84eACbOHcB3Dh5Af86eA/+I3AA/2eSTv/8/fv/+vv4//X48v////////////z++v+jupj/AGwA/z15Gv44egH/N3cB2zd3Afs3dwH/O3gP/yNwAP9nkk//+vv5///////X4NL/eZ5i/7vLsv//////+vz4/2aSTP8lcQD/O3kP/zd3Afs3dwH7N3cB/zt4D/8jcAD/ZpJN//39/P/4+vb/ToQp/wBkAP8AaAD/1N/O//////+pvaD/AGQA/0F7IP83dwH7N3cB2zh6Af86eA/+I3AA/2OQSf/+//3/7/Ps/zV3AP9JfTT/AGYA/8PSu///////uce1/wBgAP5EfiX/OHcB3Dh2AJs6fgH/O3kQ+yNxAP9olEz/+vv4//////+Nqn7/AF4A/2WRSf/u8uv//////5Wwhv8AaQD7QoEb/zh3AJw3dgA4OnkL/y5zAP5OgTf+7fHp/////////////P76/9jj0v/x9e7//////+Tr3/88fAD+NXUA/jl5B/83dgA4AAAAADt5D5gyfQD/UIE5+d7m2P7l7N//pLuY/63Bov/4+vb/+Pn3/8/byP9gjkf+IHAA+UCCE/82dgCXAAAAAAAAAABAgAAEN3cDujqAAP8pdQD+KHYA+wVtAP4AaQD/O3oA/02BNf4AbQD7JXAA/kCCFP81dgC6M2YABQAAAAAAgAACAAAAADNmAAU4dgKXOHgM/zx+Ev8+fBj/P3od/zJ1AP8udgD/QYAe/zx6Ef82dwCYQIAABAAAAAAAgAACAAAAAACAAAIAAAAAAAAAADt7Fzg6eAqbOHcC3Dd3Afs5eAr7OngN2zh4BZs3dgA4AAAAAAAAAAAAgAACAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAoAAAAEAAAACAAAAABACAAAAAAAAAEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACAAAIAAAAAAAAAADx5EzdGfCiaQHsg2jd3Avs3dwD7NncB3DZ2Aps3dgA4AAAAAAAAAACAgAACAAAAAICAAAIAAAAAAFUAAzl3CJg0dwD/AHAA/wBuAP82dwD/OHcD/zh6AP86fgH/OHkB/zh2AJdAgAAEAAAAAICAAAIAAAAAQIAABDl4Crs2fwD/Rn4l/ounffqFonj9PHkT/zN1AP83dwH9NncA+jd3Af48gQH/N3cBu1VVAAMAAAAAAAAAADh2ApdDhBv/FG0A+GmTU/7///3/9vjz/1CCNv83dwb/R30s/z15Ff82dgD+NncB+DuBAf83dwCYAAAAADd2ADg4eQH/Pnka/hZtAP5pklP//v79//X39P9BeyD/AF8A/wBnAP8cbwD/P3od/zd2AP43dgD+OHkB/zh5ADc2dgKbOn4B/zt4D/sjcAD/ZZFM//3+/f/z9fH/Z5NM/6e7nv+rvqL/bJRX/wBrAP8d)
![Zendesk](https://img.shields.io/badge/Zendesk-Support-03363D?logo=zendesk)

## 🎯 Overview

This 2.0 system imports Zendesk users, enriches them with AI-powered research, scores them from 0–10, and pushes only high‑quality B2B leads into Pipedrive.
Leads are stored in an n8n Data Table, reviewed via a web dashboard, and synchronized to Pipedrive either in daily batches or on‑demand via a webhook.

**Problem solved:** You no longer need to manually export, clean, research and qualify Zendesk users before creating organizations, people, deals and notes in Pipedrive.

## ✨ Key Features

- **Zendesk JSONL Import** – Upload exported Zendesk users (JSON/JSONL) via the dashboard
- **Email Domain Filtering** – Drops free/personal email providers (gmail, outlook, yahoo, etc.) on import
- **AI Lead Enrichment** – Google Gemini + web search agent generates decision, reasoning, shipping volume, logistics type and lead score
- **Scoring & Queueing** – Only leads with decision `YES` and score \> 5 are queued
- **Batch & Webhook Push** – Daily scheduled push at 21:00 plus a `/push-to-pipedrive` webhook for on‑demand pushes
- **Pipedrive Sync** – Automatically creates Organization, Person, Deal and Note and writes the IDs back to the Data Table
- **Dashboard UI** – Rich dashboard with filters, sorting, pagination, modal detail view, and a KVS configuration tab
- **Error Notifications** – Optional global error workflow that emails detailed failure reports

## 🏗️ High‑Level Architecture

```text
Zendesk Users (export JSONL)
        │
        │  (Upload via dashboard → /save-raw-zendesk-data)
        ▼
┌────────────────────────────────────┐
│  Data Table: verpakkingenxl-2.0   │
│  (queued / processed leads)       │
└────────────────────────────────────┘
        │
        │  AI Analysis (Main-2.0 workflow)
        ▼
Queued + Scored Leads (decision YES, score > 5)
        │
        │  Daily Schedule 21:00  +  Webhook POST /push-to-pipedrive
        ▼
Pipedrive (Organization, Person, Deal, Note)
        │
        │  GET /verpakkingenxl-2.0
        ▼
Browser Dashboard (dashboard-code.html from Dashboard-2.0)
```

## 🔧 Workflow Components

### 1. Dashboard-2.0 – Lead Dashboard & Import

**Purpose:** Serves the HTML dashboard, loads configuration (KVS) and lead data, and handles Zendesk JSONL imports.

- **Endpoint:** `GET /verpakkingenxl-2.0`
- **Nodes (core):**
  - `Dashbord Webhook` – Entry point that exposes `/verpakkingenxl-2.0`
  - `Get KVS` + `Aggregate KVS` – Load key–value configuration (prompts, limits)
  - `Get All Data` / `Aggregate Zendesk Data` – Load Zendesk leads from the `verpakkingenxl-2.0-zendesk` table
  - `Dashboard Code` – Embeds `dashboard-code.html` and injects both KVS and Zendesk data into `window.kvsDataFromN8n` and `window.zendeskDataFromN8n`
  - `Return Dashbord Code` – Returns HTML to the browser

**Dashboard tabs:**

- **📊 Dashboard**
  - Filters by search, status (queued/processed), estimated shipping volume, logistics type, and lead score range
  - Shows customer name, email, phone, shipping volume, logistics type, lead score, status and created date
  - For processed leads:
    - Status cell shows **Processed** as a link to the Pipedrive deal (if `deal_id` is present)
    - Customer name becomes a link to the Pipedrive organization (if `org_id` is present)
  - For queued leads:
    - Shows a green **Push to Pipedrive** button which calls the `/push-to-pipedrive` webhook and updates the row when IDs are returned

- **📥 Import Data**
  - Accepts `.jsonl` / `.json` files exported from Zendesk
  - Filters out free/personal email domains on the client side before saving
  - Provides search + delete per row, and “Save data for processing” button
  - On save, POSTs the cleaned user list to `/save-raw-zendesk-data`

- **⚙️ KVS Configuration**
  - UI for editing KVS keys used by the workflows:
    - `system_prompt_base_agent`
    - `system_prompt_web_search_agent`
    - `pipedrive_push_limit`
    - `daily_processing_limit`
  - Saves configuration by POSTing to `/update-kvs-2.0`

### 2. Zendesk Import Workflow (Dashboard-2.0)

**Purpose:** Accepts cleaned Zendesk user data from the dashboard and stores it in the main Data Table.

- **Endpoint:** `POST /save-raw-zendesk-data`
- **Flow (simplified):**
  1. `Zendesk Webhook` – Receives an array of Zendesk users
  2. `Loop Over Items` – Iterates over each user
  3. `Check If Already Exists` – Looks up `zendesk_id` in `verpakkingenxl-2.0-zendesk`
  4. `If No Match` – Only proceed when no existing row is found
  5. `Insert Raw Zendesk Data` – Writes a new row with:
     - `zendesk_id`, `customer_name`, `email`, `phone`, `time_zone`, `locale`
     - `status = "queued"`
     - `is_searched = false`
  6. `Return Success` – Responds `{ "status": "success" }` to the dashboard

### 3. Main-2.0 – AI Scoring & Pipedrive Sync

This workflow has two major responsibilities: AI enrichment (scoring) and pushing qualified leads to Pipedrive.

#### 3.1 AI Enrichment & Lead Scoring

- **Core nodes:**
  - `Aggregate Prompts` – Loads prompts from KVS
  - `AI Agent` (`@n8n/n8n-nodes-langchain.agent`) – Base agent that:
    - Receives customer info from Zendesk (name, email, domain, phone, time zone, locale)
    - Uses the `system_prompt_base_agent` prompt
    - Produces a structured `output` object
  - `Google Gemini Chat Model` – Backing LLM for the agent
  - `Gemini Search` (`httpRequestTool`) – Tool for web research using Gemini with `google_search`
  - `Structured Output Parser` – Ensures the agent output matches:

    ```json
    {
      "decision": "YES or NO",
      "reason": "short one-sentence justification",
      "estimated_shipping_volume": "low | medium | high",
      "likely_logistics_type": "parcels | pallets | both | unknown",
      "score": 0.0,
      "compact_instruction": "company summary"
    }
    ```

  - `If a Good Lead` – Checks `output.decision == "yes"` and `output.score > 5`
  - Data table update nodes – Write back AI results into `verpakkingenxl-2.0-zendesk`, including:
    - `decision`, `reason`, `estimated_shipping_volume`, `likely_logistics_type`, `lead_score`
    - A compact summary / note
    - `is_searched = true`

#### 3.2 Daily / Webhook Push to Pipedrive

- **Triggers:**
  - `Schedule Trigger For Pushing Data into PipeDrive` – Daily at 21:00 (Europe/Berlin)
  - Webhook: `POST /push-to-pipedrive` (same logic as the schedule, but for one‑off pushes from the dashboard)

- **Selection logic:**
  - `Get All Data` – Reads from `verpakkingenxl-2.0-zendesk` with filters:
    - `is_searched = true`
    - `status = "queued"`
  - `Sort` – Orders by `lead_score` descending
  - `Get Push Limit` (from KVS) + `Limit` – Restricts batch size based on `pipedrive_push_limit`
  - `Loop Over Items` – Iterates over the selected leads

- **Pipedrive creation:**
  - `Create Organization` – Creates an organization with custom fields populated from AI output and Zendesk fields
  - `Create Person` – Creates a person linked to the organization
  - `Create Deal` – Creates a deal linked to person + organization; sets pipeline & stage
  - `Create Note` – Creates a pinned note containing AI summary / note

- **Write‑back:**
  - A Data Table `update` node writes back:
    - `org_id`, `person_id`, `deal_id`, `note_id`
    - `status = "processed"`
  - When called via the `/push-to-pipedrive` webhook, the workflow also returns:

    ```json
    {
      "org_id": 123,
      "person_id": 456,
      "deal_id": 789,
      "note_id": 1011
    }
    ```

### 4. Notify-On-Error-2.0 – Global Error Notifications

**Purpose:** Catches workflow failures and emails a formatted error report.

- Triggered by n8n’s Error Trigger for all workflows
- Sends an HTML email containing:
  - Workflow name
  - Node that failed
  - Error message
  - Direct link to the failed execution
- Requires SMTP credentials configured in n8n

### 2. Batch Processing Workflow

**Purpose:** Pushes qualified leads to Pipedrive on a schedule.

**Trigger:** Daily at 21:00 (9:00 PM) Netherlands time

**Process:**
1. Fetches batch size limit from KVS configuration table
2. Retrieves all leads with status = "queued"
3. Sorts by lead_score (highest first)
4. Limits to configured batch size
5. Loops through each lead:
   - Creates Organization in Pipedrive
   - Creates Person (contact)
   - Creates Deal (pipeline stage 1)
   - Creates Note (AI summary + order history)
6. Updates lead status to "processed"
7. Stores Pipedrive IDs in database

### 2. Dashboard Workflow

**Purpose:** Provides web interface for monitoring and configuration.

**Endpoint:** `GET /verpakkingenxl-2.0`

**Features:**
- Real-time lead monitoring with filters
- Status tracking (queued/processed)
- Location and score filtering
- Sortable data table with pagination
- Lead detail modal popups
- KVS configuration editor

### 5. KVS Update Workflow

**Purpose:** Updates system configuration via dashboard.

**Endpoint:** `POST /update-kvs`

**Updates:**
- AI system prompts
- Batch size limits
- Other configuration parameters

### 6. Error Notification Workflow

**Purpose:** Global error handler that automatically sends email alerts when any workflow fails.

**Trigger:** Error Trigger (catches failures from all workflows)

**Process:**
1. **Error Trigger** - Detects when any workflow execution fails
2. **Edit Error Message** - Formats error details into styled HTML email with:
   - Workflow name that failed
   - Error message from the failed node
   - Name of the node that caused the failure
   - Direct link to the execution details
3. **Notify User** - Sends email notification via SMTP

**Email Template Features:**
- Mobile-responsive HTML design
- Professional styling with clear error highlighting
- System tag: "verpakkingenxl – Lead Processing System"
- Monospace formatting for technical details
- Direct link to view full execution in n8n

**Configuration Required:**
- SMTP credentials in n8n
- Update `fromEmail` and `toEmail` in the "Notify User" node

**Note:** This workflow acts as a safety net for the entire system, ensuring you're immediately notified of any issues in the lead processing pipeline.

### Required Credentials in n8n

Configure these in n8n's credential manager:

- **Pipedrive API** (Query Auth)
  - Parameter: `api_token`
  - Value: Your Pipedrive API token

- **Google Gemini API**
  - API Key from Google Cloud Console

- **SMTP Account** (for error notifications)
  - Host: Your SMTP server
  - Port: Usually 587 or 465
  - Username: Your email address
  - Password: Your email password or app-specific password
  - Secure: False

## 🚀 Installation & Setup

### Step 1: Import Workflows

1. Clone this repository:
```bash
git clone https://github.com/anas-farooq8/verpakkingenxl-2.0.git
cd verpakkingenxl-2.0
```

2. Import workflows into n8n:
   - Open n8n interface
   - Go to Workflows → Import from File
   - Import each JSON file from `/workflows` folder

### Step 2: Create Data Tables

Create two data tables in your n8n instance:

#### Table 1: `verpakkingenxl-2.0-zendesk`

Main Zendesk lead database with columns:

| Column Name | Type | Description |
|------------|------|-------------|
| zendesk_id | String | Unique Zendesk user identifier (Primary Key) |
| customer_name | String | Customer or company name |
| email | String | Email address |
| phone | String | Phone number |
| time_zone | String | Zendesk time zone |
| locale | String | Zendesk locale (e.g. "nl") |
| status | String | queued/processed |
| decision | String | YES/NO (AI decision) |
| reason | Text | AI evaluation summary |
| estimated_shipping_volume | String | low/medium/high |
| likely_logistics_type | String | parcels/pallets/both/unknown |
| lead_score | Number | Lead score 0–10 |
| compact_instruction | Text | Short company summary / instruction |
| note | Text | HTML note text pushed to Pipedrive |
| org_id | String | Pipedrive Organization ID |
| person_id | String | Pipedrive Person ID |
| deal_id | String | Pipedrive Deal ID |
| note_id | String | Pipedrive Note ID |
| is_searched | Boolean | Whether AI research has been run |
| createdAt | DateTime | Record creation timestamp |
| updatedAt | DateTime | Last update timestamp |

#### Table 2: `verpakkingenxl-2.0-KVS`

Configuration key-value store:

| Column Name | Type | Description |
|------------|------|-------------|
| key | String | Configuration key (Primary Key) |
| value | Text | Configuration value |

**Required Keys:**
- `system_prompt_base_agent` - AI prompt for base agent
- `system_prompt_web_search_agent` - AI prompt for search agent
- `pipedrive_push_limit` - Max leads to push to Pipedrive per run (stringified number)
- `daily_processing_limit` - Max leads to AI-process per day (stringified number)

### Step 3: Configure Credentials

1. Open each workflow in n8n
2. Update credential references:
   - Pipedrive API nodes → Select your Pipedrive credential
   - Google Gemini nodes → Select your Gemini credential
   - SMTP nodes (in Error Notification workflow) → Select your SMTP credential

3. Configure Error Notification workflow:
   - Open the "Notify-On-Error" workflow
   - Update the "Notify User" node:
     - Set `fromEmail` to your sender email address
     - Set `toEmail` to the admin/recipient email address
   - Activate the workflow

### Step 4: Setup Pipedrive Custom Fields

1. Go to Pipedrive → Settings → Data fields → Organization
2. Create custom fields and note their IDs:

| Field Name | Field Type | Example ID |
|-----------|-----------|-----------|
| Zendesk ID | Text | 1a654f5d... |
| Total Orders | Numeric | ae01b186... |
| Paid Orders | Numeric | 0a516666... |
| Total Value | Monetary | a785a890... |
| Lead Score | Numeric | e62dba18... |
| Estimated Shipping Volume | Text | 13096dc6... |
| Logistics Type | Text | 5df1b60a... |
| CoC Number | Text | 7e89f763... |
| VAT Number | Text | c1b3f8b6... |

3. Update field IDs in workflow nodes:
   - Open "Create Organization" node
   - Replace field IDs with your actual IDs
   - Repeat for "Update Organization" node

### Step 5: Configure Pipeline Settings

1. Get your Pipedrive pipeline ID and first stage ID:
   - Go to Pipedrive → Settings → Pipelines
   - Note the pipeline ID and first stage ID

2. Update in workflow:
   - Open "Create Deal" node
   - Set `pipeline_id` and `stage_id`

### Step 6: Webhooks in 2.0

In version 2.0 there is **no Lightspeed webhook**. Data enters the system via:
- Zendesk export (JSON/JSONL) uploaded through the dashboard
- Optional `/push-to-pipedrive` webhook, used only for pushing already‑qualified leads from the queue into Pipedrive.

### Step 7: Initialize KVS Configuration

1. Populate the KVS table with initial values:

```sql
-- Example prompts (customize for your business)
INSERT INTO "verpakkingenxl-2.0-KVS" (key, value) VALUES 
('system_prompt_base_agent', 'You are a B2B lead qualification expert...'),
('system_prompt_web_search_agent', 'You are a web research specialist...'),
('pipedrive_push_limit', '50'),
('daily_processing_limit', '200');
```

2. Or use the dashboard to configure via UI

### Step 8: Test the System

1. **Test Webhook:**
   - Trigger the `/push-to-pipedrive` webhook with a queued, AI‑processed Zendesk lead
   - Check n8n execution log
   - Verify database entry

2. **Test AI Research:**
   - Ensure a new company triggers AI workflow
   - Check AI decision and score in database

3. **Test Batch Processing:**
   - Manually trigger the scheduled workflow
   - Verify leads appear in Pipedrive
   - Check all 4 records created (Org, Person, Deal, Note)

4. **Test Dashboard:**
   - Access dashboard URL
   - Verify lead data displays correctly
   - Test KVS configuration updates

5. **Test Error Notifications:**
   - Manually trigger a workflow failure (e.g., invalid credentials)
   - Verify you receive an email notification
   - Check email formatting and execution link

## ⚙️ Configuration

### AI Prompts

Customize the AI behavior by editing the system prompts in the KVS table:

**Base Agent Prompt Example:**
```
You are a B2B lead qualification expert for a packaging company. 
Analyze the provided company information and determine if they are 
a good fit for our business.

Evaluate based on:
- Company size and shipping volume potential
- Industry relevance (e-commerce, manufacturing, retail)
- Geographic location and market presence
- Legitimacy and business maturity

Provide:
1. Decision: YES or NO
2. Score: 0-10 (where 10 is highest priority)
3. Detailed reasoning for your decision
```

**Web Search Agent Prompt Example:**
```
You are a web research specialist. Given a company name and details,
search the internet to find:
- Company size and employee count
- Business model and products/services
- Shipping and logistics needs
- Market presence and reputation
- Industry and sector information

Return concise, factual information that helps evaluate the company
as a potential B2B customer for packaging supplies.
```

### Batch Processing

Adjust the number of leads processed daily:

```sql
UPDATE "verpakkingenxl-2.0-KVS" 
SET value = '50' 
WHERE key = 'pipedrive_push_limit';
```

### Scheduling

Modify the batch processing time:
1. Open the "Schedule Trigger" node
2. Change the cron expression or time
3. Save workflow

## 📊 Usage

### Monitoring Leads

Access the dashboard at: `https://your-n8n-instance.com/webhook/verpakkingenxl-2.0`

**Dashboard Features:**
- **Filters:**
  - Status: All, Queued, Processed
  - Location: Filter by city/country
  - Lead Score: Minimum score threshold

- **Lead Table:**
  - Sortable columns
  - Pagination (20 records per page)
  - Click row for detailed view

- **KVS Configuration Tab:**
  - Edit AI prompts
  - Adjust batch size
  - Save changes via POST request

## 🗂️ Data Structure

### Lead Processing States
### Pipedrive Record Structure

**Organization:**
- Name, address, contact details
- Custom fields: metrics, IDs, scores
- Linked to Person

**Person:**
- Contact name, email, phone
- Label: "B2B Contact"
- Linked to Organization

**Deal:**
- Title: "New Business Lead – [Company Name]"
- Pipeline: Stage 1
- Source: Zendesk
- Linked to Organization and Person

**Note:**
- AI qualification summary
- Complete order history
- Lead score and reasoning
- Pinned to Deal

## 🐛 Troubleshooting

### Webhook Not Receiving Data

**Symptoms:** No executions when the `/push-to-pipedrive` webhook is called

**Solutions:**
1. Verify the workflow exposing `/push-to-pipedrive` is activated
2. Check workflow is activated
3. Use "Get All Webhooks" node to verify registration
4. Test with webhook URL directly using Postman

### AI Research Failing

**Symptoms:** Leads stuck in processing, no AI decision

**Solutions:**
1. Verify Google Gemini API credentials
2. Check API quota limits
3. Review system prompts for errors
4. Check n8n execution logs for API errors

### Leads Not Appearing in Pipedrive

**Symptoms:** Status shows "queued" but no CRM records

**Solutions:**
1. Verify Pipedrive API token is valid
2. Check custom field IDs match your Pipedrive setup
3. Verify pipeline and stage IDs are correct
4. Manually trigger batch workflow to check errors
5. Review Pipedrive API rate limits

### Duplicate Records in Pipedrive

**Symptoms:** Same company appears multiple times

**Solutions:**
1. Check if `zendesk_id` is being stored correctly
2. Verify duplicate check logic is working
3. Clear and rebuild database if corrupted
4. Check for multiple webhook registrations

### Dashboard Not Loading

**Symptoms:** 404 or blank page

**Solutions:**
1. Verify dashboard workflow is activated
2. Check webhook URL is correct
3. Review data table connections
4. Check browser console for JavaScript errors

### Error Notifications Not Sent

**Symptoms:** Workflows fail but no email received

**Solutions:**
1. Verify Error Notification workflow is activated
2. Check SMTP credentials are configured correctly
3. Verify `fromEmail` and `toEmail` are set in "Notify User" node
4. Check spam/junk folder for notification emails
5. Test SMTP connection with a simple email node
6. Review email server logs for delivery issues
7. Ensure firewall/network allows SMTP connections
