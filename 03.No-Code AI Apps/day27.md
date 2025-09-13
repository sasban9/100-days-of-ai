Great choice — Day 27 is where you **build a “Blog Summarizer” app in Bubble**. Let’s break it into a clear, guided plan so you don’t get stuck.

---

## 🔎 **Day 27: Build a Blog Summarizer App in Bubble**

**Goal:** Create a simple web app where a user pastes a blog link or text, clicks a button, and gets a concise AI-generated summary.

---

### Step 1: Set up the project

1. Log in to Bubble and create a **new app**.
2. Name it something simple like *“BlogSummarizerAI.”*
3. Choose the **blank app template** (cleaner to start).

---

### Step 2: Design the UI

1. On the main page, add:

   * A **multiline input box** → placeholder: “Paste your blog article text here.”
   * A **button** → label: “Summarize.”
   * A **text element** → to display the output summary.
2. Keep the layout simple (center everything).

---

### Step 3: Connect OpenAI API

1. Go to **Plugins tab → Add plugins → API Connector.**
2. Click *Add API*. Name it “OpenAI.”
3. Add an API call:

   * Method: POST
   * URL: `https://api.openai.com/v1/chat/completions`
   * Headers:

     * `Authorization: Bearer YOUR_API_KEY`
     * `Content-Type: application/json`
   * Body (JSON):

     ```json
     {
       "model": "gpt-4o-mini",
       "messages": [
         {"role": "system", "content": "You are a blog summarizer."},
         {"role": "user", "content": "<blog_text>"}
       ],
       "temperature": 0.3,
       "max_tokens": 300
     }
     ```
   * Replace `<blog_text>` dynamically with the input box value.

---

### Step 4: Create the workflow

1. Select the **Summarize button** → “Start/Edit Workflow.”
2. Add action → Plugins → “Call OpenAI API.”
3. For the input, pass the text from the **multiline input box.**
4. Save the response as a “Custom State” or directly display in the **Text element.**

---

### Step 5: Test

1. Preview the app.
2. Paste a blog post or article (you can copy from Medium).
3. Hit “Summarize.”
4. You should see a clean summary.

---

### Step 6: Polish

1. Add a **loading spinner** while waiting for the AI.
2. Add styling: rounded input, colored button, clean font.
3. Optional: Add a dropdown → “Summary length” (short / medium / detailed). Map this to a system prompt change.

---

### Step 7: Stretch Goals

* Add a **URL input** → auto-fetch article content with a plugin like *LinkPreview API* before summarizing.
* Store past summaries in Bubble’s database → users can log in and view their history.
* Let users export summary as PDF (Bubble plugin).

---

By the end of Day 27, you’ll have a **working AI-powered web app** that anyone can use to condense long-form content into quick summaries.

---

Do you want me to expand this into a **step-by-step Bubble editor walkthrough with screenshots-style instructions** (like “click here, then here”), so it feels like a tutorial you can follow screen-by-screen?
