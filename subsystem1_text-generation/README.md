# Dialogue generation with LLMs

In this exercise, our goal is to get familiar with basic LLM prompting, compare different available models, 
explore the limitations of LLMs, as well as to generate entertaining stories and communication scenarios 
for the final demo.

To get familiar with the basics of prompt engineering, we recommend you follow this short course: 
https://learn.deeplearning.ai/login?redirect_course=chatgpt-prompt-eng

You can also refer to this tutorial for a basic introduction/overview: https://www.promptingguide.ai/
You can use ChatGPT, Bard, or any of the LLMs available here Chat with Open Large Language Models 
https://chat.lmsys.org/ to generate text in this assignment. You can also compare different models’ subjective 
performance.

## Creating a story
First, let us start with creating a plot, or a context, for your demo. You can use well-known topics of 
general interest such as articles on scientific subjects, news, etc, to create a story based on it by 
referring the model to sources of knowledge. You can also explore the models’ “reasoning” capabilities 
through chain-of-thought prompting to derive conclusions based on the provided context. You can then 
explore factual correctness of the generated text by asking the model to compare it to other publicly 
available knowledge sources that you originally did not provide. Through iterative prompting, you can 
collaborate with the model on writing the story.

## Introducing characters and creating a dialogue
Now that we have set up the basic story, you can introduce different characters and speech styles by 
describing your characters and their demeanor in the prompts and referring to the story you created as 
the context to turn it into a dialogue. You can, for example, refer to well-known fictional movie 
characters or public figures to make the model mimic their style, or create your own characters by giving 
examples using few-shot prompting.

## Exploring the limitations of LLMs
Some main challenges around using LLMs today include possible biases, unethical and inappropriate 
responses, and factual incorrectness. In particular, while ChatGPT has powerful guardrails making it
avoid giving illegal and unethical responses, with some prompt engineering it is still possible to bypass 
them. Explore the limitations to get a better idea of the current limitations (and possibly a more creative 
demo)
