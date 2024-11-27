# Groq Chatbot

## Project Overview

Groq Chatbot is a conversational AI built using **Groq's AI models** integrated with **Streamlit** for a user-friendly interface. The app allows users to interact with the chatbot in a variety of conversational styles (personas), including a **friendly assistant**, an **expert**, and a **creative problem-solver**. The chatbot can remember previous messages and is customizable, making it adaptable for various use cases.

### Features:
- **Customizable Personas**: Choose from different conversational styles such as friendly, expert, or creative.
- **Conversational Memory**: The chatbot can remember past conversations, providing context-aware responses.
- **Model Selection**: Select from multiple Groq AI models based on your preference.
- **User Interface**: An intuitive Streamlit-based UI with easy navigation for settings, chat history, and chat statistics.
- **Clear Chat History**: Users can clear their chat history or start a new topic at any time.
- **Chat Statistics**: Track the number of messages exchanged and the duration of the conversation.

---

## Technologies Used

- **Streamlit**: A powerful tool for building interactive web applications.
- **Groq AI**: The backend AI model responsible for generating chatbot responses.
- **LangChain**: Used for managing conversational memory and integrating the AI model.
- **Python**: The programming language used to write the application logic.

---

## Getting Started

### Prerequisites

- Python 3.x
- Groq API Key (obtain from Groq)
- Required libraries (listed below)

### Installation

1. Clone this repository to your local machine.

   ```bash
   git clone https://github.com/arya-io/groq-chatbot.git
   cd groq-chatbot

2. Install the required libraries:

    ```bash
    pip install -r requirements.txt
    ```

3. Get your Groq API key from Groq and add it to the code.

    Replace `groq_api_key = ""` with your actual API key in the code.

4. Run the Streamlit app:

    ```bash
    streamlit run app.py
    ```

5. Open the app in your browser (usually at http://localhost:8501).

## How It Works

### Model Selection:
Choose from the available AI models:
- `llama3-70b-8192`
- `gemma2-9b-it`
- `mixtral-8x7b-32768`

### Persona Setup:
Select one of the available conversation styles:
- **Default**: A friendly, approachable assistant.
- **Expert**: A knowledgeable, technical assistant.
- **Creative**: An imaginative and outside-the-box thinker.

### Memory Settings:
Adjust the memory length (how many past messages the AI will remember) to fit your needs.

### Conversational Memory:
The chatbot remembers previous messages, helping it provide more context-aware responses.

### Start a New Topic:
If you want to change the conversation context, simply click the “New Topic” button to clear the memory.

## Project Structure

The project is organized as follows:
```bash
groq-chatbot/
│
├── app.py              # Main Streamlit application file
├── requirements.txt    # List of Python dependencies
└── README.md           # Project documentation (you're reading this!)
```

- **app.py**: The core of the application that includes all the Streamlit UI and interaction logic.
- **requirements.txt**: Lists all the required dependencies for the project.

## Customization

You can easily customize the chatbot by modifying the following:

- **Personas**: You can add or change the conversational styles in the `get_custom_prompt()` function.
- **AI Models**: Choose or add new models in the model selection dropdown within the sidebar.
- **Memory Length**: Adjust the slider to control how many messages the chatbot remembers.

## Contributing

We welcome contributions! If you'd like to improve or extend the functionality, feel free to open an issue or submit a pull request.

1. Fork the repository.
2. Clone your fork to your local machine.
3. Create a new branch (`git checkout -b feature-branch`).
4. Make your changes and commit them (`git commit -m 'Add feature'`).
5. Push to your fork (`git push origin feature-branch`).
6. Submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **Streamlit**: For providing an easy-to-use framework for building web applications.
- **Groq**: For providing powerful AI models that power the chatbot.
- **LangChain**: For simplifying the memory management and model chaining.
