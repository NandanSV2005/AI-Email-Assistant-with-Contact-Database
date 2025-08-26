# 🤖 AI Email Assistant Agent  

An **AI-powered assistant** built with **n8n** that interacts with users via chat, understands their intent, and automatically sends emails on their behalf.  
The agent is designed to be **friendly, professional, and helpful**, ensuring that all generated emails are clear, polite, and well-formatted.  

It also integrates with a **Contact Database**, allowing the assistant to fetch recipient details such as email addresses. This ensures flexibility, as users don’t always need to provide complete information.  

---

## 📌 Workflow Overview  

The workflow consists of the following components:  

1. **When Chat Message Received**  
   - Workflow trigger node.  
   - Starts whenever a new message is received from the user in the chat interface.  

2. **AI Agent**  
   - The central brain of the workflow.  
   - Uses the **OpenAI Chat Model** for natural language understanding and response generation.  
   - Maintains context with **Simple Memory**.  
   - Can call external tools such as:  
     - **Contact Database** → Retrieves recipient details like email addresses.  
     - **Send Email Tool** → Sends the final formatted email.  

3. **OpenAI Chat Model**  
   - Interprets the user’s query.  
   - Generates structured responses for email drafting.  

4. **Simple Memory**  
   - Retains past conversation history.  
   - Ensures that the agent remembers context (e.g., recipient name, subject, previous discussion).  

5. **Contact Database**  
   - Retrieves contact details such as email addresses from a stored sheet or database.  
   - If only a name is provided, the agent uses this tool to look up the correct email.  

6. **Send Email Tool**  
   - Sends the composed email through Gmail integration.  
   - Handles subject, recipient, and body formatting.  

7. **Edit Fields**  
   - Manual checkpoint to review and modify the generated email before sending.  

---

## ✨ Features  

- 💬 **Conversational AI** → Understands and responds naturally.  
- 🧠 **Memory Retention** → Maintains context across conversations.  
- 📧 **Automated Email Drafting & Sending** → Creates well-formatted, professional emails.  
- 📂 **Contact Database Lookup** → Automatically fetches recipient email addresses.  
- 🛠️ **Manual Review Option** → Emails can be edited before sending.  
- 🤝 **Friendly & Professional Tone** → Ensures clarity, politeness, and professionalism.  

---

## 🚀 Example Use Cases  

1. **Meeting Reminders**  
   - *User*: “Send an email to Sarah reminding her about the meeting tomorrow at 3 PM.”  
   - *Process*: The agent checks the contact database for Sarah’s email, drafts a polite reminder, and sends it.  

2. **Professional Requests**  
   - *User*: “Draft an email to my professor requesting an extension for my assignment.”  
   - *Process*: The agent generates a formal email, retrieves the professor’s email if missing, and sends it.  

3. **Follow-up Emails**  
   - *User*: “Send a thank-you email to the client after today’s call.”  
   - *Process*: The AI drafts a professional thank-you email and sends it via Gmail.  

---

## 🛠️ Tech Stack  

- **n8n** → Workflow automation platform.  
- **OpenAI Chat Model** → Natural language understanding and response generation.  
- **Simple Memory** → Conversation context retention.  
- **Contact Database (Google Sheets / Database)** → Recipient info storage & lookup.  
- **Gmail Integration** → Sending formatted emails.  

---

## 📖 How It Works  

1. The user sends a message in chat (e.g., *“Send an email to John about the project update”*).  
2. The **AI Agent** interprets the request using the **OpenAI Chat Model**.  
3. If the recipient’s email is not provided, it queries the **Contact Database**.  
4. The agent drafts the email with a greeting, body, and closing.  
5. The draft goes through the **Edit Fields** node for review.  
6. The **Send Email Tool** dispatches the email via Gmail.  
7. The user receives confirmation once the email is sent successfully.  

---

## 📌 Summary  

This project shows how an **AI-powered assistant** can simplify communication by automating email drafting and sending. With **context retention, contact lookup, and Gmail integration**, users only need to describe their intent in natural language, and the assistant takes care of the rest.  

This workflow can serve as a foundation for building:  
- 🧑‍💼 Personal assistants  
- 💼 Business communication bots  
- 📞 Customer support automation  
- 📧 Productivity tools for automated emailing  

---

## Images
<img width="1918" height="831" alt="image" src="https://github.com/user-attachments/assets/8cd6dec9-4722-4eaf-b23d-738b3096da97" />
<img width="1918" height="835" alt="image" src="https://github.com/user-attachments/assets/e3755056-d86e-4f4e-89a3-31488fdea187" />


