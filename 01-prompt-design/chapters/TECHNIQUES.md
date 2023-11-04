# Modern Prompt Design

## Introduction

In the digital age, leveraging the capabilities of large language models like OpenAI's GPT series has become increasingly popular. Crafting effective prompts for these models is crucial to obtaining desired outputs. This course aims to teach software developers the art and science of prompt design.

In this overview of modern techniques, the context is that a person who loves history wants to write a paper on the history of American Imperialism for publication.

## Multi-personas Prompting

### Description

By assigning a multiple, distinct personas to the model, we can better tailor its responses. This might include a specific job role, tone, or knowledge base.

### Benefits

- Provides a clear context to the model.
- Achieves consistent tone and style.

### Example

"You are a historian specializing in American foreign policy and a high school history teacher explaining American Imperialism to students. How would you describe the key motives, events, and figures in American Imperialism to a class of high school students, keeping in mind their need for both context and engagement?"

## Chain-of-Thought Prompting

### Description

This involves asking sequential questions or providing statements to guide the model's output in stages, instead of a single broad question.

### Benefits

- Breaks down complex queries into manageable chunks.
- Encourages more precise answers.

### Example

"Begin by defining imperialism and its general implications. Then, proceed to explore the historical context in which American Imperialism started. What were the significant wars, policies, and ideologies that characterized American Imperialism? List them in chronological order and describe the outcomes of each phase in the expansion of the United States."

## Chain-of-Thought Factored Decomposition Prompting

### Description

A deeper version of the chain-of-thought technique. Here, we deconstruct the main query into several sub-questions.

### Benefits

- Gains in-depth understanding of a subject.
- Avoids overwhelming the model.

### Example

"To understand American Imperialism, break it down into the following components: economic motivations, military motivations, cultural motivations, and political motivations. For each factor, provide historical examples and discuss their impact on American policies and foreign relations during the late 19th and early 20th centuries."

## Skeleton-of-Thought Prompting

### Description

Provide a structured outline for the model to fill in details.

### Benefits

- Gets structured and organized responses.
- Suitable for detailed explanations or content creation.

### Example

"Construct a timeline for the history of American Imperialism, starting with the purchase of Alaska and ending with the Cold War. Your timeline should include the following sections: territorial acquisitions, wars fought for imperialistic reasons, policy doctrines for expansion, and opposition to imperialism within the United States."

## Flipped Interaction Prompting

### Description

Reverse the roles. Instead of asking the model to answer, instruct the model to ask questions based on given information.

### Benefits

- Encourages deeper exploration.
- Useful for brainstorming and ideation.

### Example

"Consider yourself a journalist interviewing a panel of experts on American Imperialism. What five probing questions would you ask to elicit their views on the positive and negative aspects of American Imperialism? Use their responses to create a comprehensive article that explores the complexity of the topic."

## Self-reflection Prompting

### Description

Ask the model to introspect its responses or correct/improve previous outputs.

### Benefits
- Refines model's output.
- Addresses any ambiguities.

### Example

"Write a critical essay on the history of American Imperialism. After your initial draft, self-reflect on the content: Does your essay comprehensively cover the timeline and motivations? How does it address the various viewpoints and cultural impacts? Then, revise the essay to ensure it provides a balanced and thorough examination of American Imperialism."
