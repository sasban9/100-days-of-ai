Great choice — Day 15 is where you build a super practical AI-powered workflow: **Zoom/Google Meet transcript → AI summary → stored for later use.** This is the kind of automation that instantly saves time and looks impressive in your portfolio. Let’s break it down step by step.

---

# **Day 15 Expanded: Meeting Notes Automation**

### 🎯 Goal

Every time you have an online meeting, the transcript (or recording notes) should automatically be summarized by AI and saved in a place you can easily access later (like Google Docs, Notion, or Slack).

---

### 🔧 Tools You’ll Use

* **Zoom** or **Google Meet** (source of transcript)
* **Zapier** or **Make** (automation platform)
* **OpenAI or Claude API** (summarization)
* **Google Docs / Notion / Slack** (final destination)

---

### 🛠️ Step-by-Step Setup

1. **Get Meeting Transcript**

   * Zoom → enable “Save transcript” in your account settings.
   * Google Meet → use **Otter.ai** or **Meet Transcripts** extension to auto-capture.

2. **Create Trigger in Zapier/Make**

   * Trigger = “New file in Google Drive / New transcript saved.”
   * This ensures automation starts as soon as a transcript appears.

3. **Send Transcript to AI**

   * Add a step in Zapier: “Send text to OpenAI (ChatGPT API)”
   * Prompt example:

     ```
     Summarize this meeting transcript into 3 sections: 
     1. Key decisions made 
     2. Action items with owners 
     3. Questions or unresolved issues
     ```
   * Test with a small transcript to confirm formatting.

4. **Save the Summary**

   * Step 1: Create new Google Doc titled “Meeting Notes - \[Date]”.
   * Step 2: Insert AI summary inside.
   * Optional: Also post to Slack channel #meeting-summaries.

5. **Test End-to-End**

   * Run one short meeting (or upload dummy transcript).
   * Make sure the whole chain works: transcript → AI → summary → stored.

---

### 🌟 Stretch Goals (Level-Up)

* **Auto-tagging:** Add metadata (Project Name, Meeting Type) using AI.
* **Email automation:** Email summary to all meeting participants.
* **Notion Integration:** Send summaries into a Notion database with columns (Date, Team, Key Points).
* **Multi-language:** Ask AI to also generate a version in Hindi/French/Spanish for global teams.

---

### 📌 Deliverable by End of Day 15

* A **working automation** that captures meeting transcripts → summarizes with AI → saves in Google Docs/Notion/Slack.
* A **short Loom demo** showing how it works (add to your portfolio).

---

⚡ Quick thought: Do you want me to also **write out the exact Zapier workflow with all steps and sample prompts** so you can just copy-paste it, or would you prefer a more flexible blueprint where you choose the storage tool (Google Docs, Notion, or Slack)?
