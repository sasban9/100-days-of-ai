Great question — Day 35 is when you **add voice capability to your chatbot in Voiceflow**. This step turns your chatbot from just a text-based tool into something far more natural and engaging — like Alexa, Siri, or a customer support agent that can actually “talk.” Here’s how you’d approach it:

---

### 🎯 **Goal for Day 35**

Take your existing **AI customer support bot** (from Day 34) and make it capable of real conversation with **speech input + output**.

---

### 🛠️ **Steps**

1. **Enable Voice in Voiceflow**

   * Voiceflow allows you to design both text-based and voice-first experiences.
   * In your project settings, select a **Voice Assistant flow** instead of just a Chat flow.
   * Add **Speak blocks** where the bot should respond out loud instead of just showing text.

2. **Connect to a Speech-to-Text (STT) service**

   * By default, Voiceflow supports integrations with Google Speech-to-Text or Amazon Transcribe.
   * This converts user speech into text → feeds it into your AI bot.

3. **Add Text-to-Speech (TTS)**

   * For responses, connect to Amazon Polly, ElevenLabs, or Google Cloud TTS.
   * This way, your chatbot doesn’t just “print” the response but actually **speaks** it out.

4. **Design Voice-Friendly Flows**

   * Shorten AI responses so they’re easy to listen to (people won’t wait through a 500-word answer).
   * Add reprompting flows (“Sorry, could you repeat that?”).
   * Insert natural pauses with SSML tags (`<break time="500ms"/>`).

5. **Test on Real Device**

   * Voiceflow lets you preview right in the browser.
   * For extra polish, connect your bot to Alexa or Google Assistant and test with an actual device.

---

### 💡 **Pro Tips**

* Use **ElevenLabs** for more natural voices if you want your bot to sound human-like.
* Add **emotion control** (e.g., friendly, serious) in TTS settings for customer support vs. fun use cases.
* Record a short demo: Ask your bot a question and capture the voice response → this makes for a great **portfolio piece** and LinkedIn post.

---

### 🌟 **Example Use Case**

Imagine you’re building an **AI receptionist for a clinic**.

* A patient says: “I want to book an appointment.”
* The bot uses STT to understand → checks schedule (API) → replies with TTS:
  “Sure, I found an opening next Tuesday at 4 PM. Would you like me to book it?”

That feels **way more human** than typing back and forth.

---

Would you like me to expand this further into a **step-by-step mini project guide** (with example flows + code snippets for TTS/STT) so that Day 35 becomes a complete hands-on workshop?
