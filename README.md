# AI-Content-Detector
Tool using AWS Bedrock Service - Llama 3.1 405B
- to give **AI generated score**, 
- to **analyze and explain** how much input text is AI generated.

## Motivation
- I created post in **Dev.to** and discuss how to eliminate COMPLETELY AI Generated Posts. 
  - https://dev.to/omerberatsezer/why-should-we-keep-writing-lets-discuss-2nc
- After discussion in the post, I decided to create a simple SAMPLE AI Content Detector tool with **PROMPT TEMPLATE** to show that it's really **SIMPLE and EFFECTIVE**.
- I mentioned this app in the following DEV.to post, please have a look for details, and please leave your valuable ideas in the post's comment:
  - https://dev.to/omerberatsezer/open-source-ai-content-detector-app-with-aws-bedrock-to-separate-completely-ai-vs-human-generated-2de4 

## Run
```shell
git clone https://github.com/omerbsezer/AI-Content-Detector
pip install -r requirements.txt
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

## Detected Patterns - Analysis
### AI Score for Human Generated Text in App
![mydevto-post-score-analysis](https://github.com/omerbsezer/AI-Content-Detector/blob/main/gif/mydevto-post-score-analysis.png)

### AI Score for COMPLETELY AI Generated Text
![image](https://github.com/user-attachments/assets/0eab6388-46e8-4869-aa22-4bbe4edf8715)

![image](https://github.com/user-attachments/assets/963c9fb0-2e75-499a-bc62-39f9f28079db)

