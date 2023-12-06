# Introduction to Retrieval Augmented Generation

Recall that two major weaknesses of language models are the tendency to hallucinate and a training cutoff. If you ask a language model a question for which it cannot know the answer and press it enough, it is liable to hallucinate an answer.

These language models also have a training cutoff. For example, ChatGPT 3.5 has a cutoff of January 2022 so asking about anything beyond that date can either result in an incorrect response or a refusal answer.

For example, try the following prompt:

> How did Amazon's sales change in 2022?

This information was not included in the training data, so the language model is not able to give an answer. 

Even if we ask for something it could know, it is uncertain how much that answer can be trusted.

> How did Amazon's sales change in 2020?

You may get an answer, but it is not clear if it is factual or just sounds plausible. In addition, if you ask follow-up questions, you'll quickly find that the model is unable to answer.

> How much of Amazon's 2020 net sales came from North America?