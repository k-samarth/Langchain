# Langchain

### Introduction
LangChain is a framework for developing applications powered by language models. 

Large Language Models don't store state. Instead, they try to predict: 
> P(next token | prompt)

That is finding the probability of the next token given the prompt.
LLMs are great at generating something new from scratch or via conditional generation based on input prompt(text)

The problem that arises when we use LLMs alone is that they can't use the traditional software stack like other applications.
**LLMS doesn't store state, and each call to the large language model is individual. Conversation state needs to be passed back to the model each time. Also, we are constrained by the token span size.**

#### LLM is a tool that allows us to interact with the normal software stack like APIs, Tools and Data Sources.

### Prompt
> Prompting is making the model generate texts conditioned on an input text.

#### Parts of Prompt
> #### Context
> prompt = """ You are a digital assistant who helps users create business names based on descriptions of businesses. You provide short catchy names.

> #### Examples
> \- Examples -<br>
> Dan's Mechanic shop for repairs -> Dan's Auto
> A Greek restaurant specializing in lamb -> Aegean Lamb Hut
> A Vietnamese sandwitch shop -> Saigon Sandwitch
> A luxury wedding planner -> Fab Weddings

> #### Tasks
> What is good name for {biz_description}?

> #### Output
> Name:""" 
