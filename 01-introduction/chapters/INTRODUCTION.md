# Introduction to Prompt Design

## What is a Large Language Model?

## What You Can Use It For

**Generating Text**

LLMs are designed and trained for generating language, and so are naturally great at generating coherent text. Try this prompt:

> Write a riddle involving a llama.

You can be very specific about the text generated. For example,

> Write a riddle involving a llama which doesn't reference South America.

Where LLMs really shine is when you need to generate a lot of ideas very quickly. Try this one:

> Give me 5 puns involving penguins.

One nice thing about working with a large language model is that it won't get annoyed if you keep changing what you ask for or ask for more ideas.

> Give me 10 more.

It is very good at getting you unstuck or providing an outline or an idea.

> Give me some ideas for writing an article about bike safety. 

**Summarizing Text**

LLMs can do very well at summarizing text.

> Summarize this text in 3 or fewer sentences: "Nashville is the capital and most populous city of the U.S. state of Tennessee, as well as the seat of Davidson County. With a population of 689,447 at the 2020 U.S. census,[d] Nashville is the 21st most-populous city in the United States, and the fourth most populous city in the southeastern U.S.[6] Located on the Cumberland River,[8] the city is the center of the Nashville metropolitan area, and is one of the fastest growing in the nation.[9][10]
>
> Named for Francis Nash, a general of the Continental Army during the American Revolutionary War, the city was founded in 1779. The city grew quickly due to its strategic location as a port on the Cumberland River and, in the 19th century, a railroad center. Nashville as part of Tennessee seceded during the American Civil War; in 1862 it was the first state capital in the Confederacy to be taken by Union forces. After the war, the city reclaimed its stature and developed a manufacturing base.
>
> Since 1963, Nashville has had a consolidated city-county government, which includes six smaller municipalities in a two-tier system. The city is governed by a mayor, a vice-mayor, and a 40-member metropolitan council; 35 of the members are elected from single-member districts, while five are elected at-large. Reflecting the city's position in state government, Nashville is home to the Tennessee Supreme Court's courthouse for Middle Tennessee, one of the state's three divisions.
>
> Nashville is considered a global city type "Gamma" by the GaWC as of 2020.[11] A major center for the music industry, especially country music, Nashville is commonly known as "Music City".[12] It is home to three major professional sports teams, the Predators, Titans, and Nashville SC. The city is also the home of many colleges and universities including Tennessee State University, Vanderbilt University, Belmont University, Fisk University, Trevecca Nazarene University, and Lipscomb University. Nashville is sometimes referred to as the "Athens of the South" due to the large number of educational institutions.[13] The city is also a major center for the healthcare,[14] publishing,[15] banking,[16] automotive,[17] and technology[18] industries. Entities with headquarters in the city include AllianceBernstein,[19] Asurion,[20] Bridgestone Americas,[21] Captain D's,[22] Concord, Hospital Corporation of America,[23] LifeWay Christian Resources,[24] Logan's Roadhouse,[25] and Ryman Hospitality Properties.[26] "

**Improving Writing**

LLMs can be used to improve an existing piece of writing.

> Please help make this more persuasive: "Regular exercise is important for overall health. You should be exercising throughout the week to improve cardiovascular health, lower blood pressure, and decrease inflammation."

You can even use a series of prompts to further refine or improve.

> Make it less formal. Target it to teens and young adults.

Keep experiementing to see what output you get.

> Add a second paragraph.

> Write it in the style of Ernest Hemingway.

**Writing From Different Perspectives**

> Give me a fictional transcript of a conversation between Ferdinand Magellan and Neil Armstrong.

## What You Can't Use It For

LLMs are not a substitute for a search engine. One major limitation is that there is a training cutoff. ChatGPT 3.5's training data, for example, stops at January 2022.

> Where is First Republic Bank located?

A major limitation to LLMs is that they are prone to **hallucinations**, where a language model will, quite confidently present incorrect information as fact. This can come in the form of plausible-sounding but inforrect information or sometimes information unrelated to the given context. Try the following prompt. You should get some very reasonable-sounding quotes, and some of the may actually be real. But a lot of them will be completely made up.

> I want to write a short story about Nashville. Please give me 10 quotes about Nashville with attribution to help inspire me as I write.

Also, ChatGPT tends to be bad at math. Try the following and other basic arithmetic questions, and you'll quickly find that ChatGPT will make very basic errors. Keep in mind that a large language model is not a calculator and will make errors, so you should always double-check its logic.

>  Is 10456 divisible by 17?

Why do these happen? LLMs are models designed to generate text. They are not reasoning engines. Therefore, it is important to recognize these inherent limitations so that you can avoid them or improve your prompting to work around them.