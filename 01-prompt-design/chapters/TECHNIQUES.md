# Modern Prompt Design

## Introduction

In the digital age, leveraging the capabilities of large language models like OpenAI's GPT series has become increasingly popular. Crafting effective prompts for these models is crucial to obtaining desired outputs. This course aims to teach software developers the art and science of prompt design.

## Multi-personas Prompting

### Description

By assigning a multiple, distinct personas to the model, we can better tailor its responses. This might include a specific job role, tone, or knowledge base.

### Benefits

- Provides a clear context to the model.
- Achieves consistent tone and style.

### Example

Prompt: "As a murder detective, explain the steps to investigate a crime scene. Also take on the role of a murderous criminal and how you could avoid getting caught during each one of those steps."

## Chain-of-Thought Prompting

### Description

This involves asking sequential questions or providing statements to guide the model's output in stages, instead of a single broad question.

### Benefits

- Breaks down complex queries into manageable chunks.
- Encourages more precise answers.

### Example

First prompt: "Who is Sherlock Holmes?"
Second prompt: "What methods does he use to solve mysteries?"


## Chain-of-Thought Factored Decomposition Prompting

### Description

A deeper version of the chain-of-thought technique. Here, we deconstruct the main query into several sub-questions.

### Benefits

- Gains in-depth understanding of a subject.
- Avoids overwhelming the model.

### Example

- Main Prompt: "Describe the ecosystem of a rainforest."
- Sub-questions:
  - "What is the climate of a rainforest?"
  - "Name the primary layers of a rainforest"
  - "What animals can be found in the canopy layer?"

## Skeleton-of-Thought Prompting

### Description

Provide a structured outline for the model to fill in details.

### Benefits

- Gets structured and organized responses.
- Suitable for detailed explanations or content creation.

### Example

Prompt: "Fill in the details for the lifecycle of a butterfly: 1) Egg, 2) Larva, 3) Pupa, 4) Adult."

## Flipped Interaction Prompting

### Description

Reverse the roles. Instead of asking the model to answer, instruct the model to ask questions based on given information.

### Benefits

- Encourages deeper exploration.
- Useful for brainstorming and ideation.

### Example

- Information: "Volcanoes are geological formations."
- Prompt: "Ask five questions about volcanoes."

## Self-reflection Prompting

### Description

Ask the model to introspect its responses or correct/improve previous outputs.

### Benefits
- Refines model's output.
- Addresses any ambiguities.

### Example

- First prompt: "Explain the water cycle."
- Second prompt: "Reflect on your previous answer and provide a more concise explanation."
- Third prompt: "Then determine if the more concise explanation is sufficient for a beginner to understand."

