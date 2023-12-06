# Providing Context

We have already seen that language models are very good at summarizing text and extracting useful information out of a given passage. We can use this to our advantage when trying to get a language model to answer a question for us. 

For example, let's ask about the previous question, but provide some potentially useful context from Amazon's 2021 10-K:

> How did Amazon's sales change in 2022? Use the following to answer: 
>
> Net Sales
>Net sales include product and service sales. Product sales represent revenue from the sale of products and related shipping fees and digital media content where we record revenue gross. Service sales primarily represent third-party seller fees, which includes commissions and any related fulfillment and shipping fees, AWS sales, advertising services, Amazon Prime membership fees, and certain digital content subscriptions. Net sales information is as follows (in millions):
>											
>  
>	Year Ended December 31,
> 	2021		2022
>Net Sales:			
>North America	$	279,833 			$	315,880 	
>International	127,787 			118,007 	
>AWS	62,202 			80,096 	
>Consolidated	$	469,822 			$	513,983 	
>Year-over-year Percentage Growth (Decline):			
>North America	18 	%		13 	%
>International	22 			(8)	
>AWS	37 			29 	
>Consolidated	22 			9 	
>Year-over-year Percentage Growth, excluding the effect of foreign exchange rates:			
>North America	18 	%		13 	%
>International	20 			4 	
>AWS	37 			29 	
>Consolidated	21 			13 	
>Net sales mix:			
>North America	60 	%		61 	%
>International	27 			23 	
>AWS	13 			16 	
>Consolidated	100 	%		100 	%
>Sales increased 9% in 2022, compared to the prior year. Changes in foreign currency exchange rates reduced net sales by $15.5 billion in 2022. For a discussion of the effect of foreign exchange rates on sales growth, see “Effect of Foreign Exchange Rates” below.
>North America sales increased 13% in 2022, compared to the prior year. The sales growth primarily reflects increased unit sales, including sales by third-party sellers, advertising sales, and subscription services. Increased unit sales were driven largely by our continued focus on price, selection, and convenience for our customers, including from our shipping offers.
>International sales decreased 8% in 2022, compared to the prior year, primarily due to the impact of changes in foreign currency exchange rates, partially offset by increased unit sales, including sales by third-party sellers, advertising sales, and subscription services. Increased unit sales were driven largely by our continued focus on price, selection, and convenience for our customers, including from our shipping offers. Changes in foreign currency exchange rates reduced International net sales by $15.0 billion in 2022.
>AWS sales increased 29% in 2022, compared to the prior year. The sales growth primarily reflects increased customer usage, partially offset by pricing changes, primarily driven by long-term customer contracts.
>

We can also further utilize the language model's ability to summarize.

> Make your answer 3 sentences or less.