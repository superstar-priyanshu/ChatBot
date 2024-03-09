Simple Chatbot

This project consists of a basic chatbot that leverages a JSON-based knowledge base to respond to user queries. The chatbot is designed to find the best match for a user's question within its knowledge base and provide the corresponding answer. If the chatbot cannot find an appropriate response, it prompts the user to teach it a new response, thereby expanding its knowledge base.

Features

Knowledge Base Management: Load and save a dynamic knowledge base stored in a JSON file.
Question Matching: Utilize the difflib library to find close matches between the user's question and existing questions in the knowledge base.
Learning Capability: Ability to learn new questions and answers from user input, enhancing its utility over time.
Interactive Interface: A simple and interactive command-line interface for users to ask questions and teach the chatbot.
How It Works

Load Knowledge Base: At startup, the chatbot loads its knowledge base from a specified JSON file, containing predefined questions and answers.
User Interaction: Users can ask questions through the command-line interface. The chatbot attempts to find the best match for the question within its knowledge base.
Providing Answers: If a close match is found, the chatbot responds with the corresponding answer. Otherwise, it asks the user to provide a new answer, updating its knowledge base accordingly.
Knowledge Base Update: New questions and answers provided by users are added to the knowledge base and saved to the JSON file for future use.
Setup

Installation: Ensure you have Python installed on your system. Clone this repository or download the source code.
Dependencies: This project uses standard Python libraries. No additional installation is required.
Running the Chatbot: Navigate to the project directory and run the script using Python:
bash
Copy code
python chat_bot.py
Interacting with the Chatbot: Simply type your question in the command line and press Enter. Type "quit" to exit the chatbot interface.
Extending the Knowledge Base

The chatbot's knowledge base is stored in a file named knowledge.json. You can pre-populate this file with questions and answers to enhance the chatbot's utility. The file should follow this format:

json
Copy code
{
  "questions": [
    {
      "question": "Your question here",
      "answer": "Your answer here"
    },
    ...
  ]
}
Feel free to contribute to this project by improving the chatbot's functionality or expanding its knowledge base.
