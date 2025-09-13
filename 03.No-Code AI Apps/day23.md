Great — let’s zoom in on **Day 23: Add login/signup to your Bubble app**. At this stage, you’ve already built a simple input → AI response app (Day 22), and now you’re making it feel like a *real* product by adding user authentication.

---

### 🎯 Goal for Day 23

Transform your simple Bubble app into a personalized tool where users can sign up, log in, and save their data.

---

### 🔹 Step 1: Understand Why Login/Signup Matters

* Lets users create an account → their data, history, or preferences can be saved.
* Adds professionalism → real-world apps almost always have authentication.
* Prepares your app for monetization → gated access, subscriptions, or tiered usage.

---

### 🔹 Step 2: Bubble’s Built-in User System

Bubble already has a **User data type**. Every time someone signs up, Bubble creates a new User entry in the database. You don’t need to code anything complex.

---

### 🔹 Step 3: Adding Signup

1. In your Bubble editor, drag a **Signup/Login Popup** from Bubble’s pre-made elements.
2. Add **Input fields**: email, password.
3. Add a **Signup button** → create workflow → “Sign the user up.”
4. Bubble will automatically encrypt and store user credentials.

---

### 🔹 Step 4: Adding Login

1. Reuse the same popup or create a new **Login form**.
2. Add email + password input fields.
3. Add a **Login button** → workflow → “Log the user in.”
4. Add a condition: if login fails, show an error message.

---

### 🔹 Step 5: Adding Logout

1. Add a button in your app’s header → workflow → “Log the user out.”
2. Test that once logged out, the user can’t access protected pages.

---

### 🔹 Step 6: Protecting Pages

* Go to page settings → under “Page is visible only when…” add condition: *Current User is logged in*.
* Redirect users who aren’t logged in back to login/signup.

---

### 🔹 Step 7: Saving Personalized Data

Once users log in, you can tie AI responses or app actions to their accounts.

* Example: store “Chat history” as a data type linked to *Current User*.
* Now each user sees *only their history* when logged in.

---

### 🔹 Step 8: Testing

1. Sign up with a test email.
2. Log out, log in again, make sure data persists.
3. Try with two different accounts → confirm isolation of data.

---

### 🔹 Step 9: Optional Enhancements (if time permits)

* Add **Google login** with Bubble’s OAuth plugin.
* Add **Password reset flow**.
* Add **Profile page** where users can update their info.

---

### 🔹 Deliverable for Day 23

* A working login/signup/logout flow.
* User data is stored separately.
* At least one feature (like saved chat history) personalized per user.

---

### 🔹 Demo Idea

Record a 1-minute Loom video:

1. Sign up with new account.
2. Show how AI app remembers/saves data.
3. Log out → log in → data still there.

That video becomes portfolio proof that you can build real apps with authentication.
