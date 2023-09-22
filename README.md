# An-app-to-review-feedback-for-a-product

## Goals
In the context of building a demo application for app review feedback from the Apple Store, I have developed a user interface (UI) that effectively gathers both rating and review data. This UI incorporates three crucial functions provided through Gradio output, namely sentiment analysis, summarization, and entity extraction.

- Entity extraction: involves identifying and extracting specific entities or information from a given review data
- Sentiment - the overall positive or negative sentiment of each review data
- Summary - generate a summary of the review data

## Flow
<img width="651" alt="flow" src="https://github.com/jmin-39/An-app-to-review-feedback-for-a-product/assets/85851625/0253d3ee-0879-427e-8274-c632ade01e8a">
<br/> 
<br/> 
1. Creating a Crawler Function to Scrape Apple App Store App Reviews and Ratings Using Python in a Jupyter Notebook in a Local Environment. <br/> 
2. Requesting the Crawler as Input Data. <br/> 
3. Loading the GPT Model from OpenAI. <br/> 
4. Prompt Engineering for Sentiment Analysis, Entity Extraction, Summarization, and Rating. <br/> 
5. Building an App UI using Gradio.

## Prompt Engineering
### Few-shot prompts
### 1. Entity extraction 
```python
prompt = "Extract entities (e.g., names, locations, dates) from the following text:"
```
### 2. Sentiment
```python
prompt = "Classify the review text into negative or positive."
```
### 3. Summary
```python
prompt = "It's nice that they support English, but the menus are a bit strange in English. I wish I could set the language within the app.
    Explain the above in one sentence:"
```

## Build an App UI with Gradio
* Gradio Public link: https://5f9d920f62dbcfc2c5.gradio.live
<img width="1050" alt="App UI" src="https://github.com/jmin-39/An-app-to-review-feedback-for-a-product/assets/85851625/6d92561f-1a0b-4f3d-a55f-88dca8b246ac">

* Sample App UI
<img width="1047" alt="Sample App UI" src="https://github.com/jmin-39/An-app-to-review-feedback-for-a-product/assets/85851625/9b586051-4af6-49af-bb43-dda7baec13e4">


## Next steps
- Due to capacity issues with the local LLM model, I opted to use LLM GPT for the project.
- The necessity of fine-tuning with review data

## References
- https://apps.apple.com/us/app/youtube-watch-listen-stream/id544007664](https://apps.apple.com/us/app/%EC%BF%A0%ED%8C%A1%EC%9D%B4%EC%B8%A0-%EB%B0%B0%EB%8B%AC%EC%95%B1/id1445504255
- https://github.com/IBM/watson-discovery-ui
- https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/
