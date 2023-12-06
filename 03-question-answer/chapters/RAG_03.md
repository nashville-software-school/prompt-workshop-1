# Providing the Most Relevant Context

The question now is how do we provide useful context but in a way that doesn't require us to manually provide the context? One solution is **Retrieval Augmented Generation**. The idea is to search through the possible context and extract out the passages that are most semantically similar to the posed query. 

To see this in action, you can follow along in [the accompanying Google Colab notebook](https://colab.research.google.com/drive/1hRxMZz4bnTEi3uybVnhiNIgpgzj89uV5?usp=sharing). 

>Use the following pieces of context to answer the question at the end. If you don't know the answer, just say that you don't know, don't try to make up an answer.
>In our opinion, Amazon.com, Inc. (the Company) 
>maintained, in all material respects, effective internal control over 
>financial reporting as of December 31, 2022, based on the COSO 
>criteria.
>Changes in foreign currency exchange rates reduced International net 
>sales by $15.0 billion in 2022.AWS
> sales increased 29% in 2022, compared to the prior year.
>Net sales information is as follows (in millions):  Year Ended December 31, 20212022Net Sales:North America$279,833 $315,880 International127,787 118,007 AWS62,202 80,096 Consolidated$469,822 $513,983 Year-over-year Percentage Growth (Decline):North America18 %13 %International22 (8)AWS37 29 Consolidated22 9 Year-over-year Percentage Growth, excluding the effect of foreign exchange rates:North America18 %13 %International20 4 AWS37 29 Consolidated21 13 Net sales mix:North America60 %61 %International27 23 AWS13 16 Consolidated100 %100 %Sales
> increased 9% in 2022, compared to the prior year.
>Herrington has served as CEO Worldwide Amazon Stores since July 2022, 
>Senior Vice President, North America Consumer from January 2015 to July 
>2022, and Senior Vice President, Consumables from May 2014 to December 
>2014.Brian T. Olsavsky. Mr.
>Actual 
>results and outcomes could differ materially for a variety of reasons, 
>including, among others, fluctuations in foreign exchange rates, changes
> in global economic conditions and customer demand and spending, 
>inflation, interest rates, regional labor market and global supply chain
> constraints, world events, the rate of growth of the Internet, online 
>commerce, and cloud services, the amount that Amazon.com invests in new 
>business opportunities and the timing of those investments, the mix of 
>products and services sold to customers, the mix of net sales derived 
>from products as compared with services, the extent to which we owe 
>income or other taxes, competition, management of growth, potential 
>fluctuations in operating results, international growth and expansion, 
>the outcomes of claims, litigation, government investigations, and other
> proceedings, fulfillment, sortation, delivery, and data center 
>optimization, risks of inventory management, variability in demand, the 
>degree to which we enter into, maintain, and develop commercial 
>agreements, proposed and completed acquisitions and strategic 
>transactions, payments risks, and risks of fulfillment throughput and 
>productivity.
>These forward-looking 
>statements reflect Amazon.coms expectations as of February 2, 
>2023, and are subject to substantial uncertainty.
>The sales 
>growth primarily reflects increased customer usage, partially offset by 
>pricing changes, primarily driven by long-term customer contracts.Operating Income (Loss) Operating income (loss) by segment is as follows (in millions):Year Ended December 31,20212022Operating Income (Loss)North America$7,271 $(2,847)International(924)(7,746)AWS18,532 22,841 Consolidated$24,879 $12,248 Operating
> income was $24.9 billion and $12.2 billion for 2021 and 2022.
>Increased unit sales were driven largely by our continued focus on 
>price, selection, and convenience for our customers, including from our 
>shipping offers.23Table of ContentsInternational
> sales decreased 8% in 2022, compared to the prior year, primarily due 
>to the impact of changes in foreign currency exchange rates, partially 
>offset by increased unit sales, including sales by third-party sellers, 
>advertising sales, and subscription services.
>The
> increase in AWS operating income in absolute dollars in 2022, compared 
>to the prior year, is primarily due to increased sales and cost 
>structure productivity, including a reduction in depreciation and 
>amortization expense from our change in the estimated useful lives of 
>our servers and networking equipment, partially offset by increased 
>payroll and related expenses and spending on technology infrastructure, 
>all of which were primarily driven by additional investments to support 
>AWS business growth.
>AMAZON.COM, INC.By:/s/ Andrew R. JassyAndrew R. JassyPresident and Chief Executive OfficerPursuant
> to the requirements of the Securities Exchange Act of 1934, this Report
> has been signed below by the following persons on behalf of the 
>registrant and in the capacities indicated as of February 2, 2023.
>...
>
>Question: How did Amazon's sales change in 2022?
>Helpful Answer:
>


Once you have the vector database set up, you can use it to ask any question that you like.

Another example:

>Use the following pieces of context to answer the question at the end. If you don't know the answer, just say that you don't know, don't try to make up an answer.
>For 
>example, we face a number of open investigations based on claims that 
>aspects of our operations violate competition rules, including aspects 
>of Amazons U.S. and European marketplace for sellers, particularly with
> respect to use of data, fulfillment services, and featured offers, and 
>legislative and regulatory initiatives in Europe and elsewhere allow 
>authorities to restrict or prohibit certain operations or actions 
>pre-emptively without the need to assess specific competitive effects.
>Actual 
>results and outcomes could differ materially for a variety of reasons, 
>including, among others, fluctuations in foreign exchange rates, changes
> in global economic conditions and customer demand and spending, 
>inflation, interest rates, regional labor market and global supply chain
> constraints, world events, the rate of growth of the Internet, online 
>commerce, and cloud services, the amount that Amazon.com invests in new 
>business opportunities and the timing of those investments, the mix of 
>products and services sold to customers, the mix of net sales derived 
>from products as compared with services, the extent to which we owe 
>income or other taxes, competition, management of growth, potential 
>fluctuations in operating results, international growth and expansion, 
>the outcomes of claims, litigation, government investigations, and other
> proceedings, fulfillment, sortation, delivery, and data center 
>optimization, risks of inventory management, variability in demand, the 
>degree to which we enter into, maintain, and develop commercial 
>agreements, proposed and completed acquisitions and strategic 
>transactions, payments risks, and risks of fulfillment throughput and 
>productivity.
>We 
>dispute the allegations of wrongdoing and intend to defend ourselves 
>vigorously in this matter.In
> May 2018, Rensselaer Polytechnic Institute and CF Dynamic Advances LLC 
>filed a complaint against Amazon.com, Inc. in the United States District
> Court for the Northern District of New York.
>We dispute the allegations of 
>wrongdoing and intend to defend ourselves vigorously in this matter.In
> December 2021, the Italian Competition Authority (the ICA) issued a 
>decision against Amazon Services Europe S.à r.l., Amazon Europe Core S.à
> r.l., Amazon EU S.à r.l., Amazon Italia Services S.r.l., and Amazon 
>Italia Logistica S.r.l.
>We dispute the allegations of 
>wrongdoing and will continue to defend ourselves vigorously in this 
>matter.59Table of ContentsIn
> November 2020, the European Commission issued a Statement of Objections
> alleging that Amazon uses data relating to our marketplace sellers in a
> manner that infringes EU competition rules.
>The inability to hire, train, 
>retain, and manage sufficient required personnel may limit our 
>international growth.The
> Peoples Republic of China (PRC) and India regulate Amazons and its 
>affiliates businesses and operations in country through regulations and
> license requirements that may restrict (i) foreign investment in 
>and operation of the Internet, IT infrastructure, data centers, retail, 
>delivery, and other sectors, (ii) Internet content, and 
>(iii) the sale of media and other products and services.
>We dispute 
>the allegations of wrongdoing and intend to defend ourselves vigorously 
>in this matter.Beginning
> in March 2020, with Frame-Wilson v. Amazon.com, Inc. filed in the 
>United States District Court for the Western District of Washington, 
>private litigants have filed a number of cases in the U.S. and Canada 
>alleging, among other things, price fixing arrangements between 
>Amazon.com, Inc. and vendors and third-party sellers in Amazons stores,
> monopolization and attempted monopolization, and consumer protection 
>and unjust enrichment claims.
>In addition, safety is integral to 
>everything we do at Amazon and we continue to invest in safety 
>improvements such as capital improvements, new safety technology, 
>vehicle safety controls, and engineering ergonomic solutions.
>In April 2022, BroadbandiTV alleged in its damages report that,
> in the event of a finding of liability, Amazon could be subject to $166 to $986
> million in damages.
>We dispute the allegations of wrongdoing and 
>intend to defend ourselves vigorously in these matters.In
> October 2020, BroadbandiTV, Inc. filed a complaint against Amazon.com, 
>Inc., Amazon.com Services LLC, and Amazon Web Services, Inc. in the 
>United States District Court for the Western District of Texas.
>...
>
>Question: What are the biggest challenges facing Amazon?
>Helpful Answer:
>