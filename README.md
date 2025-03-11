# AI-Content-Detector
Tool using AWS Bedrock Service - Llama 3.1 405B
- to give **AI generated score**, 
- to **analyze and explain** how much input text is AI generated.

## Motivation
- I created post in **Dev.to** and discuss how to eliminate COMPLETELY AI Generated Posts. 
  - https://dev.to/omerberatsezer/why-should-we-keep-writing-lets-discuss-2nc
- After discussion in the post, I decided to create a simple SAMPLE AI Content Detector tool with **PROMPT TEMPLATE** to show that it's really **SIMPLE and EFFECTIVE**.

## Run
```shell
python -m streamlit run .\main.py
```

### AI Score for Human Generated Text
- My Post Analysis => https://dev.to/omerberatsezer/why-should-we-keep-writing-lets-discuss-2nc

![text-devto-human-analysis](https://github.com/omerbsezer/AI-Content-Detector/blob/main/gif/text-devto-human-analysis.gif)

### AI Score for COMPLETELY AI Generated Text
![text1-analysis](https://github.com/omerbsezer/AI-Content-Detector/blob/main/gif/text1-analysis.gif)

## Structure
- **ai_generated_analyzer.py** => prompt template, parse response
- **main.py** => Streamlit GUI
  - left side => Input Text
  - right side => AI Generation Score, Evaluation, Detection Patterns 

## Tests
- Sample text under the test-input-files directory
