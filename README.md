# Customer-Voice-Call-Analytics
This project utilizes a combination of Whisper (OpenAI's speech recognition model) and an LLM (Large Language Model) to transcribe and analyze customer call audio files. The analysis provides insights such as sentiment, intent, and topics discussed during the call, along with a summary of key information. The analysis is returned in a structured JSON format.

## Features
- **Speech Recognition:** Converts customer call audio files into text using OpenAI’s Whisper model.
  
- **Language Detection:** Detects the spoken language in the audio.
  
- **Context Analysis:** Uses a Large Language Model (LLM) to analyze the transcribed text and extract:
  - **Sentiment:** Classifies segments of the conversation as Positive, Neutral, or Negative.
  - **Intent:** Detects the intent behind the conversation.
  - **Topics:** Identifies the topics discussed in the call.
  - **Summary:** Summarizes the conversation.
    
- **JSON Output:** Returns the analysis in a structured JSON format for easy consumption.



## Project Components
### 1. Whisper (Speech Recognition)
The Whisper model is used to transcribe the audio file into text. It also detects the spoken language in the audio file.

### 2. LLM (Large Language Model)
The LLM is used for analyzing the transcribed text. It breaks down the conversation and provides insights into the sentiment, intent, topics, and a summary.

### 3. LangChain
LangChain is used to create an LLM chain that processes the context (transcribed text) with custom prompts and memory to store the conversation history.

### 4. Together API
The LLM model mistralai/Mixtral-8x7B-Instruct-v0.1 is accessed through the Together API. The model is capable of analyzing large chunks of text and providing detailed analysis.

### Future Improvements
- **Support for Multiple Languages:** Extend the analysis to support multilingual transcription and sentiment analysis.
  
- **Interactive Frontend:** Develop a web-based interface to upload audio files and display analysis results.
  
- **Fine-Tuning:** Fine-tune the model to improve accuracy based on specific use cases like customer service, technical support, etc.


## Output Screenshots
![Screenshot 2024-09-11 144424](https://github.com/user-attachments/assets/b07a2c54-d5f6-433e-bf4b-8842cbfe6187)

