Great choice — let’s zoom in on **Day 12: Build your first Zap (Gmail → Google Sheet log).**

This is your first practical step into **AI-powered automation**, so the goal here is to connect a common tool you use daily (email) with structured storage (Google Sheets). By the end, you’ll have a live automation where every new email gets logged into a sheet without you lifting a finger.

---

## **Day 12 — Step-by-Step Guide**

### 1. Setup

* **Accounts needed:**

  * Gmail (or GSuite)
  * Google Sheets
  * Zapier (free account is enough for this test)
* **Create a new Google Sheet** with columns like:

  * Timestamp
  * From (Sender)
  * Subject
  * Snippet/Preview

---

### 2. Create the Zap in Zapier

1. Log in to Zapier → click **Create Zap**.

2. **Trigger app:** Choose **Gmail**.

   * Event = *New Email*
   * Connect Gmail account.
   * Filter: Only log emails that meet a condition (e.g., subject contains “Invoice” or “Job”).

3. **Action app:** Choose **Google Sheets**.

   * Event = *Create Spreadsheet Row*.
   * Connect Google Sheets.
   * Pick the sheet you created.
   * Map Gmail fields → Spreadsheet columns:

     * `Date` → Timestamp
     * `From` → Sender
     * `Subject` → Subject line
     * `Body Preview` → Snippet

---

### 3. Test & Run

* Send yourself a test email.
* Zapier should automatically insert a row in your sheet.
* You now have a **live email log**!

---

### 4. Bonus (Add AI Magic ✨)

* Insert an **AI step** (Zapier → OpenAI integration):

  * Pass the email text → get a summary or classify it.
  * Add new columns in the sheet: `AI Summary`, `Category`.
* Example prompt:

  ```
  Summarize this email in one sentence. Then classify it as "Invoice", "Personal", "Work", or "Other".
  ```
* Now your Google Sheet becomes an **AI-powered inbox dashboard**.

---

### 5. Deliverable for Day 12

* One working Zap: Gmail → Google Sheet.
* Optional: AI Summary + Category column.
* Screenshot or Loom video of the workflow running.
* Add it to your **AI Automation Portfolio** (you’ll keep building this all the way to Day 100).

---

⚡ By the end of Day 12, you’ll have taken a real manual process (checking + organizing emails) and turned it into an automated AI-supported workflow — something you can also pitch to clients later.

---

Do you want me to also design a **Day 12 “practice challenge”** where you build *two extra variations* of this workflow (one personal, one business) so you go deeper instead of just stopping at the simple email log?
