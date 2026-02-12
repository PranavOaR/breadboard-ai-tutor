# Breadboard AI Tutor Chatbot

This project is an AI-powered tutor chatbot that helps students learn breadboard experiments.

It uses:
- A structured dataset of breadboard experiments (JSON)
- Retrieval-based grounding (RAG style)
- Groq AI API (Llama 3.1) for teacher-style explanations

## Features
- Step-by-step experiment guidance 
- Component explanations (LED, resistor, buzzer, LDR, etc.)
- Troubleshooting common mistakes
- Safe responses grounded only in dataset

## Folder Structure

data/ → Experiment dataset  
notebooks/ → Colab chatbot demo  
examples/ → Sample Q&A outputs  

## Open Notebook in Google Colab

Click below to open directly:

[Open in Colab](https://colab.research.google.com/github/PranavOaR/breadboard-ai-tutor/blob/main/notebooks/breadboard_chatbot_demo.ipynb)

## Student Version Chatbot Notebook

Open the chatbot UI directly:

[Student Chatbot (Gradio UI)](https://colab.research.google.com/github/PranavOaR/breadboard-ai-tutor/blob/main/notebooks/student_chatbot.ipynb)

## AI Usage
Groq API (Llama 3.1) is used only to rewrite dataset responses into a friendly tutor style.
The chatbot is strictly grounded and does not hallucinate outside the dataset.

**Note:** The chatbot is dataset-grounded and automatically works even if Groq quota is exceeded.

## Getting Started

### Prerequisites

- Python 3.8 or higher
- pip package manager
- Groq API key (get free from [console.groq.com](https://console.groq.com))

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/PranavOaR/breadboard-ai-tutor.git
   cd breadboard-ai-tutor
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Open the demo notebook:
   ```bash
   jupyter notebook notebooks/breadboard_chatbot_demo.ipynb
   ```

## Usage

Explore the demo notebook to see the AI tutor in action. Check out the sample questions in the `examples/` folder for inspiration on what you can ask.

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests.

## License

This project is open source and available under the MIT License.
