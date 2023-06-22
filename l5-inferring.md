# Lesson5: Inferring

## Overview 

In this lesson, you will infer `sentiment` and `topics` from product reviews and news articles.

##  Inferring

`Inferring` : set of tasks where the model takes a text as input and performs some kinds of analysis.
- Ex: Extracting lables, names, understand the sentiment of text, etc

**Inferring LLM vs classical ML Model**
-  classical ML Model : 
   -  complex and slow process
   -  need of a different model for each task (extraction, sentiment analysis..)
-  LLM models : much faster and all you need is a `prompt`
   -  only need one API (model) to perform many different tasks

## Application & examples

Product review

```python
lamp_review = """
Needed a nice lamp for my bedroom, and this one had \
additional storage and not too high of a price point. \
Got it fast.  The string to our lamp broke during the \
transit and the company happily sent over a new one. \
Came within a few days as well. It was easy to put \
together.  I had a missing part, so I contacted their \
support and they very quickly got me the missing piece! \
Lumina seems to me to be a great company that cares \
about their customers and products!!
"""
```
Sentiment analysis (positive/negative)

```python
prompt = f"""
What is the sentiment of the following product review, 
which is delimited with triple backticks?

Review text: '''{lamp_review}'''
"""
response = get_completion(prompt)
print(response)
```

`Completion : `

```
The sentiment of the product review is positive.
``` 






Check out the [notebook](./lab/l5-inferring.ipynb) to see more code examples.

## References

Main course : 
- https://learn.deeplearning.ai/chatgpt-prompt-eng/lesson/5/inferring

Introducing the Hugging Face LLM Inference Container for Amazon SageMaker : 
- https://huggingface.co/blog/sagemaker-huggingface-llm

llm-inference - Kaggle
- https://www.kaggle.com/code/miwojc/llm-inference