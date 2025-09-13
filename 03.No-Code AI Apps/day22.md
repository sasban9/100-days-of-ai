Alright, let’s zoom in on **Day 22: Build a simple Bubble app: input → AI response** and expand it into a **step-by-step mini-guide** so you can actually complete this task in one sitting.

---

# 🛠️ Day 22 — Your First Bubble AI App

### 🎯 Goal

Create a no-code web app in Bubble where a user types something into a text box, clicks a button, and gets an AI-generated response displayed back.

---

### 🔹 Step 1: Set up your Bubble environment

1. Go to [bubble.io](https://bubble.io) and sign up (free plan works).
2. Create a **new app** → give it a name like *AI Playground*.
3. Pick a **blank template** (keeps things clean).

---

### 🔹 Step 2: Build the UI

In the Bubble editor:

1. Drag a **Text Input** element onto the page → label it “Your Question.”
2. Drag a **Button** element → label it “Ask AI.”
3. Drag a **Multiline Text** element → make it the response box (empty by default).

At this stage, your app looks like:
`[ Text Input ]  [ Ask AI Button ]`
`[ Multiline Text Box (AI Response) ]`

---

### 🔹 Step 3: Connect to OpenAI (or another LLM)

1. Go to **Plugins tab** in Bubble → click **Add plugins**.
2. Search for **OpenAI GPT** (official or community plugin) → install it.
3. Add your **OpenAI API key** (from [platform.openai.com](https://platform.openai.com/)).

---

### 🔹 Step 4: Build the workflow

1. Select the **Ask AI Button** → click **Start/Edit Workflow**.
2. Add an **Action** → “Plugins” → “OpenAI - Create Completion (GPT-4/GPT-3.5).”
3. In the prompt field, insert the user input: `Input's value`.
4. Set the response to update the **Multiline Text box**.

So the workflow is:

* User clicks “Ask AI” → send input text to OpenAI → display response.

---

### 🔹 Step 5: Test your app

1. Click **Preview** in the Bubble editor.
2. Type a question like: *“Write me a haiku about AI in education.”*
3. Hit **Ask AI** → response should appear in the text box.

---

### 🔹 Step 6: Polish (optional)

* Add a loading spinner while waiting for response.
* Limit input length (so users don’t overload the API).
* Add styling → background color, rounded corners, font tweaks.
* Save conversation history (input + response) in Bubble’s database.

---

### 🔹 Step 7: Share it

* Copy the **preview link** → share with a friend.
* Post a screenshot on LinkedIn/Twitter with: *“Built my first AI app on Bubble today 🚀. Ask AI anything, and it answers instantly!”*

---

✅ At the end of Day 22, you’ll have a fully working AI-powered app in Bubble that takes input and returns an AI-generated answer.