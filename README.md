# MathsGpt : Text To Math Problem Solver and Data Search Assistant

## Overview
The **Text To Math Problem Solver and Data Search Assistant** is a Streamlit-based web application that leverages the power of LangChain and Google Gemma 2 (via ChatGroq) to solve mathematical and logic-based questions, as well as provide data-driven insights using Wikipedia as a source. This application is designed to assist users in performing complex calculations, solving reasoning problems, and retrieving relevant information seamlessly.

## Features
- **Mathematical Problem Solving**: Solves arithmetic and advanced mathematical expressions using the Calculator tool powered by the LLMMathChain.
- **Logical Reasoning**: Answers logic-based and reasoning questions with detailed, step-by-step explanations.
- **Data Search**: Fetches and summarizes information from Wikipedia using the Wikipedia API Wrapper.
- **Interactive Chat**: Provides an interactive chat interface for users to input their questions and view responses in real-time.

## Installation
### Prerequisites
1. Python 3.8 or higher
2. A valid Groq API key for accessing the Google Gemma 2 model
3. Required Python libraries (listed below)

### Required Libraries
Install the required Python libraries using pip:
```bash
pip install streamlit langchain langchain_groq wikipedia-api
```

### Clone the Repository
Clone this repository to your local machine:
```bash
git clone https://github.com/your-repo/text-to-math-problem-solver.git
```

### Running the Application
1. Navigate to the project directory:
```bash
cd text-to-math-problem-solver
```
2. Run the Streamlit app:
```bash
streamlit run app.py
```
3. Open your web browser and go to the local URL displayed in the terminal (usually `http://localhost:8501`).

## Usage
1. **Enter Groq API Key**: Provide your Groq API key in the sidebar to initialize the application.
2. **Ask a Question**: Enter your question in the text area provided. This can be a mathematical problem, a logical reasoning question, or a query requiring information from Wikipedia.
3. **Get an Answer**: Click the "Find My Answer" button to generate a response. The assistant will provide detailed answers in the chat interface.

### Example Question
```
I have 5 bananas and 7 grapes. I eat 2 bananas and give away 3 grapes. Then I buy a dozen apples and 2 packs of blueberries. Each pack of blueberries contains 25 berries. How many total pieces of fruit do I have at the end?
```

## Code Overview
- **Streamlit Setup**: Configures the Streamlit page, including the title, sidebar, and user input interface.
- **Groq Integration**: Uses ChatGroq to interact with the Google Gemma 2 model for generating responses.
- **WikipediaAPIWrapper**: Wraps Wikipedia's API for efficient information retrieval.
- **LLMMathChain**: Handles mathematical computations and complex problem-solving.
- **Tools and Agent Initialization**: Combines tools (Wikipedia, Calculator, Reasoning) into a unified agent for seamless interactions.
- **Interactive Chat**: Maintains session state for user and assistant messages to provide a conversational experience.

## File Structure
```
.
├── app.py               # Main application file
├── requirements.txt     # List of required Python libraries
└── README.md            # Documentation file
```




Feel free to contribute to the project or suggest improvements!

