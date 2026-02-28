# AI Concept Explainer

A fun and interactive Python module that uses AI to explain any topic in the style of different colorful characters: **Shakespeare**, a **Pirate**, or a **Bandit**! 

This project is powered by [Groq's Llama-3.1-8b-instant](https://groq.com/) model and utilizes [LiteLLM](https://docs.litellm.ai/) for seamless API integration.

## Features
- **Multiple Personas**: Get explanations delivered in Early Modern English (Shakespeare), pirate slang, or Wild West cowboy jargon.
- **Fast and Efficient**: Uses Groq's ultra-fast inference API.
- **Interactive CLI**: Simple command-line interface to input topics and select your preferred mode.

## Prerequisites
- Python 3.7+
- A Groq API Key (get one at [console.groq.com](https://console.groq.com/))

## Installation

1. **Navigate to the project folder:**
   ```bash
   cd Module1
   ```

2. **Set up a Virtual Environment (Optional but recommended):**
   ```bash
   python -m venv venv
   # On Windows
   venv\Scripts\activate
   # On Mac/Linux
   source venv/bin/activate
   ```

3. **Install Dependencies:**
   Install the required packages using pip:
   ```bash
   pip install -r requirements.txt
   ```

4. **Environment Variables:**
   Create a `.env` file in the root directory (if it's not already there) and add your Groq API key:
   ```env
   GROQ_API_KEY=your_groq_api_key_here
   ```
   *(Note: Never share your actual API key publicly!)*

## Usage

Run the main script from your terminal:

```bash
python concept_explainer.py
```

You will be prompted to enter a topic and select a mode:
```text
Enter topic: Quantum Computing
Select mode (Shakespeare/Pirate/Bandit): Pirate
```

### Example Output (Pirate Mode)
> Arrr! Ye be a legendary pirate captain explainin' tech to yer scurvy crew!  
> Gather 'round the deck as we uncover the buried treasure of Quantum Computin'... Yo ho ho!

## Project Structure
- `concept_explainer.py`: The main entry point script that handles user input and makes the API call.
- `prompts.py`: Contains the system prompts and styling instructions for the different personas (Shakespeare, Pirate, Bandit).
- `requirements.txt`: Lists the Python dependencies (`litellm`, `python-dotenv`).
- `.env`: Stores environment variables securely.

## License
MIT License
