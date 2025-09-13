Great choice — **Day 26: Build a mini “Idea Generator” app in Glide** is where things start to feel real because you’ll build something people can actually use. Let’s expand it into a clear step-by-step guide.

---

# 🌱 Day 26 — Build a Mini “Idea Generator” App in Glide

**Goal:** Create a simple no-code app that takes a user’s input (like a topic or problem) and generates fresh ideas using AI.

---

### 1. **Set Up Glide**

* Go to [Glide](https://glideapps.com/) and create a free account.
* Start with a **blank project** (not a template) so you learn from scratch.
* Choose **Apps** (mobile-style UI) rather than **Pages** (desktop dashboards).

---

### 2. **Design the Input Screen**

* Add a **Text Entry component** for user input, label it: “Enter your topic/problem.”
* Add a **Button** below it called “Generate Ideas.”
* Connect both to a Glide table (every Glide project has a Google Sheets-like table).

---

### 3. **Set Up the AI Action**

* In Glide, open the **Actions editor** for the “Generate Ideas” button.
* Select **“OpenAI → Generate text”** (Glide has this built in).
* Prompt example:

  ```
  You are an idea generator. Suggest 5 innovative ideas for {User Input}.
  ```
* Map `{User Input}` to the text entry field.
* Save the AI response into a column called **Ideas**.

---

### 4. **Display the Results**

* Add a **Rich Text component** or **List component** to show the generated ideas.
* Bind it to the **Ideas column**.
* Style it so it looks neat (bulleted list, numbered items, etc.).

---

### 5. **Polish the UX**

* Add a fun header (e.g., “💡 Instant Idea Generator”).
* Add example placeholder text in the input field: *“Ex: social media content, startup ideas, classroom activities”*.
* Make the button stand out with a bright color.

---

### 6. **Test**

* Try inputs like:

  * “Marketing campaign for a bakery”
  * “Startup idea for reducing food waste”
  * “Fun activities for kids on a rainy day”
* See if results are relevant and useful. If not, tweak your prompt.

---

### 7. **Publish**

* Click **Share App** → get your unique Glide link.
* Share it with 2–3 friends and ask them to try it.

---

### 8. **Stretch Goal (Optional)**

* Add a **Category Picker** (e.g., Business, Education, Lifestyle) and adjust your AI prompt dynamically:

  ```
  Generate 5 creative {Category} ideas for {User Input}.
  ```
* This makes the app feel more personalized.

---

💡 **Outcome by the end of Day 26:** You’ll have a **working mobile-friendly AI app** where anyone can type a problem and instantly get fresh ideas. It’s simple but powerful — and can evolve into a niche product later.

---

Do you want me to also design a **Day 26 “Prompt Bank”** with ready-made prompts you can plug into Glide (like startup ideas, content ideas, product features), so you don’t have to write them from scratch?
