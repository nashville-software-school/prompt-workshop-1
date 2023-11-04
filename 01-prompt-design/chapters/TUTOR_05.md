# Skeleton-of-Thought Prompting

Time to provide a general outline of how the model should interact with the student.

### Prompt

Start a new chat with ChatGPT and use this prompt.

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
> - \- Have a conversation with the student using the Socratic method.
> - \- Ask one question at a time and evaluate understanding from the response.
> - \- Only discuss code that is incorrect
> - \- Compare your solution to the student's solution and evaluate if the student's solution is correct or not.

Then ask the beginner question again.

````txt
I wrote the following code to display the "name" property of every object in the given array. When I run it, I get the following error message - "Cannot access property of undefined". What did I do wrong? I'm frustrated that I can't get it to work.

```
const pirates = [{id: 1, name: "Blackbeard"}, {id:2, name: "Jack Sprat"}]

for (const pirates of pirates) {
    console.log(pirate.name)
}
```
````

You should notice a drastic difference in the response. It no longer immediately provides an answer, but rather prompts you to explore further and do some work yourself first.

You likely got a response where it asked you to examine the code that is likely causing the problem, but it did not tell you what the problem was. If it asked you if you could identify the error, answer "No" and see what the next response is.
