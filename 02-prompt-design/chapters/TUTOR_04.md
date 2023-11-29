# Chain-of-Thought Factored Decomposition Prompting

Along with the chain of thought above, provide a strategy for the tool to deconstruct what its goal is and have context.

### Prompt

Start a new chat with ChatGPT and use this prompt. You will immediately notice a difference in the response that you get.

> I want you to help beginner software developers understand the fundamentals of software. Assume the following roles.
>
> - \- An expert software mentor who can provide guidance on practical techniques
> - \- A software development instructor who understand which foundational concepts are needed
> - \- A beginner software developer that can understand the novice language used by a student
> - \- If asked a question, your job is not to provide the solution.
> - \- You must develop code for a solution yourself first. Do not show me your solution when you develop it.
> - \- Don't show the student any code until the student provides updated code that is correct.
> - \- After you have helped me understand the code and I have fixed it, do not follow up with alternative approaches
> - \- Determine which programming language is being used by analyzing the code provided.
> - \- If code isn't provided in the question, ask which programming language is being used.


Now that you have provided much more guidance, the tool is now assuming the right roles and you can ask a question and see what response you get. Ask the following software developer beginner question.

````txt
I wrote the following code to display the "name" property of every object in the given array. When I run it, I get the following error message - "Cannot access property of undefined". What did I do wrong? I'm frustrated that I can't get it to work.

```
const pirates = [{id: 1, name: "Blackbeard"}, {id:2, name: "Jack Sprat"}]

for (const pirates of pirates) {
    console.log(pirate.name)
}
```
````

While it waited for you to ask a question, the response you got immediately went into code generation mode, so it's not quite acting as a real mentor yet.

