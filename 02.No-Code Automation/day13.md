Great choice — **Day 13** is where you bring automation + AI together, which is a turning point. Let’s expand it into a **step-by-step mini-project** you can actually execute.

---

# 🌟 Day 13: Automating Email Summaries with AI

### 🎯 Goal

Set up a system where **incoming emails are automatically summarized** by ChatGPT and logged into Google Sheets (or sent to Slack/Notion). This saves time scanning long emails and helps you spot priorities fast.

---

### 🛠️ Tools Needed

* **Zapier** (or **Make.com**) → for automation
* **OpenAI API key** (get from platform.openai.com)
* **Gmail** → as trigger
* **Google Sheets / Notion / Slack** → as storage/destination

---

### 🔧 Step-by-Step Setup

**Step 1: Trigger Setup (Zapier)**

1. Go to Zapier → Create new Zap.
2. Choose **Gmail** as trigger app.
3. Trigger event: **“New Email in Inbox”** (you can filter by label, e.g., “Work” only).

**Step 2: AI Summarization**

1. Add an **“Action”** step → Choose **OpenAI**.
2. Connect your OpenAI account with API key.
3. Prompt setup:

   ```
   Summarize this email in 3 bullet points.
   Highlight:  
   - Key decision/action required  
   - Urgency (low/medium/high)  
   - Sentiment (positive/neutral/negative)  

   Email content: {{BodyPlain}}
   ```
4. Test with one real email → see summary.

**Step 3: Output Destination**
Option A: **Google Sheets**

* Add new row → Save “From”, “Subject”, “Summary”, “Urgency”.

Option B: **Slack**

* Send a Slack message to yourself or team with “New summarized email.”

Option C: **Notion**

* Create new database entry for each summarized email.

**Step 4: Testing & Tuning**

* Test with 3–5 different emails (short, long, newsletter, urgent).
* Adjust prompt for clarity (e.g., limit to 50 words, add emojis for urgency 🚨).

---

### 🚀 Stretch Goals (Optional)

* Add a filter: only summarize emails >200 words.
* Add auto-tagging (personal, work, finance).
* Add priority flagging (if “meeting” or “invoice” → mark as high priority).
* Send a daily digest of summaries at 9am.

---

### 📝 Deliverable for Day 13

* Working Zapier automation that catches emails → AI summary → logs to Sheets/Slack.
* Screenshot/video demo saved to your **Day 13 Project Log**.

---

Would you like me to also **write the exact Zapier “AI Action” prompt template** you can just copy-paste and tweak?
