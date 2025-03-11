# AI-Content-Detector
Tool using AWS Bedrock Service - Llama 3.1 405B
- to give AI generated score, 
- to analyze and explain how much input text is AI generated.

## Run
```shell
python -m streamlit run .\main.py
```

## Structure
- **ai_generated_analyzer.py** => prompt template, parse response
- **main.py** => Streamlit GUI
  - left side => Input Text
  - right side => AI Generation Score, Evaluation, Detection Patterns 

## Tests
- Sample text under the test-input-files directory