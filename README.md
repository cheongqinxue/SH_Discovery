### Information Extraction

These demos show how NER, coreferencing and SRL come together to identify people, organisations and other entities mentioned in text, and the actions or events that involve them. The specific use case here is to extract statements made by people or organisations, so SRL picks out statements made and attributes them to one of the captured entities. Each demo will display a list of captured NERs and spans in the text that refer to them. You can mouse over the unerlined text or the entities listed at the top to reveal their coreferent spans (in blue highlights) and statements captured (in bold).

- [Amazon Union Election Do-Over Recommendation Hinges on Mailbox](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Information%20Extraction%20Demos/demo_a.html)
- [USPS has shorted some workers’ pay for years](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Information%20Extraction%20Demos/demo_b.html)
- [TV best bets](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Information%20Extraction%20Demos/demo_c.html)
- [Reese Witherspoon's Hello Sunshine to Be Sold to Media Company Backed by Blackstone](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Information%20Extraction%20Demos/demo_d.html)
- ['Functionally useless': California privacy law's big reveal falls short](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Information%20Extraction%20Demos/demo_e.html)

These are the people and organizations that were captured from the entire sample set:

<p align="center">
  <img src="organizations.png" width="500">
</p>
<p align="center">
  <img src="persons.png" width="500">
</p>

#### Identifying stakeholders to investigate

Statements can be extracted and analysed in aggregate. We can figure out who was talking about an entity of interest and study the average sentiments of the statements made about that entity. Using articles in Aug 21, the following depicts the average sentiment of statements made by various persons/organisations that mention Amazon.

The Retail, Wholesale and Department Store Union's (RWDSU) statements are negative on average - not surprising since they are accusing Amazon of [wrongdoing during a union election](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Information%20Extraction%20Demos/demo_a.html).

![alt text](https://github.com/cheongqinxue/SH_Discovery/blob/main/Sentiment/fileA.png)

Similar plots studying the sentiments of statements made that mention Facebook and the United States Postal Service respectively:

![alt text](https://github.com/cheongqinxue/SH_Discovery/blob/main/Sentiment/fileF.png)
<br>
![alt text](https://github.com/cheongqinxue/SH_Discovery/blob/main/Sentiment/fileU.png)

#### How are the stakeholders related?

As it turns out, one of those in the diagram above, Stuart Appelbaum, works for the RWDSU. This information can be accumulated across several articles to create a relationship network. For RWDSU, 3 unique employees were discovered automatically:
<p align="center" style="margin:-10%;">
  <img src="Relation%20Extraction/RWDSU_1.png" width="550">
</p>

Some of the larger relationship networks discovered using the same method:<br>
<i>Note these charts are interactive. You can drag the nodes to reposition them if the labels are difficult to see</i><br>
- [Amazon](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/amazon.html)
- [AWS](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/aws.html)
- [Retail, Wholesale and Department Store Union](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/rwdsu.html)
- [American Federation of Labor and Congress of Industrial Organizations](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/AFL.html)
- [Assembly Committee on Governmental Employees](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/AssemblyCommitteeOnGovernmentalEmployees.html)
- [Global Stewardship Portfolio Construction](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/GlobalStewardshipPortfolioConstruction.html)
- [Justice Department](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/JusticeDepartment.html)
- [Michael Ray Ivory](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/MichaelRayIvory.html)
- [NY State Energy Research Development](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/NYStateEnergyResearchDevt.html)
- [Congressional Black Caucus](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/congressionalBlackCaucus.html)
- [Sentate Appropriations Committee](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/senateAppropriationsComm.html)
- [Biden](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/biden.html)
- [Trump](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/Trump.html)
- [Cori Bush](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/coribush.html)
- [Birmingham Times](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/birminghamtimes.html)
- [NY Times](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/nytimes.html)
- [League of Women Voters](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/leagueofwomenvoters.html)
- [Facebook](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/facebook.html)
- [Google](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/google.html)
- [Richard Trumka](https://htmlpreview.github.io/?https://github.com/cheongqinxue/SH_Discovery/blob/main/Relation%20Extraction/richardtrumka.html)
