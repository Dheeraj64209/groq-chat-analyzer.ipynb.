# Groq Chat Analyzer

This project demonstrates a **chat analysis system** using Groq/OpenAI API with the following features:

1. **Conversation Management with Versioned Memory**
   - Stores chat history with roles (`user`, `assistant`, `system`).
   - Maintains **versioned snapshots** after each message.
   - Supports **rollback** to any previous snapshot.
   - Automatically summarizes older conversation turns after a configurable number of messages.

2. **Message Importance Scoring**
   - Assigns scores to messages based on:
     - Emails
     - Phone numbers
     - Age mentions
     - Keywords like `signup`, `payment`, `urgent`

3. **Regex Extractors**
   - Extract emails, phone numbers, and age from chat text.

4. **Action-Item Extractor**
   - Extracts structured actionable tasks from conversations using a function-call schema.
   - Returns tasks as a JSON object for programmatic use.

5. **Demo Features**
   - Runs **multiple sample chats**.
   - Shows **all snapshot versions** of conversation memory.
   - Demonstrates **rollback to previous summary**.
   - Extracts **action items** from the final conversation.

---



## How to Use

1. Open the notebook `groq_chat_analyzer.ipynb` in **Google Colab** or Jupyter Notebook.
2. Install dependencies:


