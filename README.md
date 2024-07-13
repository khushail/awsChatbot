# AWS Bedrock Chatbot
Explains the basic way of accessing Bedrock LLMs, with chatbot framework for Q n A in Multiple languages

## Instrcution to setup this chatbot
1. Get the access to the required LLM on AWS account. For this repo, its "Anthropic- Claude model sonnet". Once you get the access, copy the Model Id and save it for future usage.
2. Get the User profile name which has access to the lLM .
3. Every model has different input parameters for setting. The claude models have this -
  
```py
  llm = BedrockChat(
    model_id=modelID,
    client=bedrock_client,
)
```
4. Input variables for the LLM are 2 -Language and Input text.
5. Mac_char input is limited to 100 chars which can be changed -
```py
freeform_text = st.sidebar.text_area(label="what is your question?",
    max_chars=100)
```
