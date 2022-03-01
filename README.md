# TwitterNetworkAnalysis-DS



<b>Introduction</b>

The political situation in Russia is continuing to be a very sensitive question not only for the Russians, but also for the external forces. Therefore, it is important to understand the balance of forces for grasping the current political situation in Russia and for the future references

Alexei Anatolievich Navalny is the first prominent opposition leader of Putin regime. He organized several demonstrations and is known to have a great impact on the youth of Russia. 

Vladimir Vladimirovich Putin is a Russian politician and former intelligence officer who is serving as the current president of Russia since 2012, previously being in the office from 1999 until 2008. Putin is the second-longest serving European president, after Alexander Lukashenko of Belarus.

The expected outcome of the research is some assumptions based on the first-hand view of the situation:

•	Alexei Navalny wins Sakharov Prize, the EU's highest award for human rights work, so most definitely it would be discussed a lot in tweets

•	September elections

•	Overall, as a citizen of Russia, I expect to find more positive opinions about Navalny than about Putin

•	Putin & his conservative view on gender problems

Thus, to comprehended more thoroughly political situation we should perform data analysis and network analysis.

<b>Data collection</b>

For data analysis, we do not need every feature that we can fetch with Twint. In fact, we need to use mostly “cleaned tweets” (from top words, hashtags, etc), which will be placed in a new column in each data frame also will help us to perform network analysis much easier.  
 

<b>Feature selection</b>

For data analysis we do not need every feature that we can fetch with Twint. In fact we need to use mostly “cleaned tweets” (from stop words, hashtags, etc), which will be placed in new column in each dataframe. This column also will help us to perform network analysis much easier. 


<b>Data analysis</b>

After we extracted and clean the data, we can get a taste of what people talking about discussing Alexei Navalny and Vladimir Putin. Word cloud is an excellent instrument for that. 

At the fig. 1 the word cloud of #Navalny tweets is shown. 

 ![image](https://user-images.githubusercontent.com/90958123/156226415-99ae68b0-2204-46c8-9dae-6bfa17878e41.png)

Fig. 1. #Navalny word cloud.


As it was predicted, Sakharov prize is quite a hot topic among the tweets, as well as his status of being in jail and topics regard his opposition’s agendas (freedom, putin critic, anti corruption).

At the fig. 2 the word cloud of #Putin tweets is shown. 

![image](https://user-images.githubusercontent.com/90958123/156226444-83bf90e2-a677-4ca6-bda1-b3c20765f736.png)

 
Fig. 2. #Putin word cloud.


Name of Vladimir Putin is mention among the line about gender crimes (as we predicted), gas, crime.

Further, we can analyze the tweet for their sentiment, to get overall mood towards two leaders. The sentiments are shown on the fig. 3 and fig. 4.

![image](https://user-images.githubusercontent.com/90958123/156226466-df07f9ce-76ae-43b0-8cac-bc572d8e58e3.png) ![image](https://user-images.githubusercontent.com/90958123/156226476-a134d3f3-8a9f-4c53-a155-b28db7defe14.png)

  
Fig. 3. Bar charts of sentiments.

From the data, we can somewhat balanced the attention of Twitter users for two leaders, but I would like to pinpoint, that despite Navalny becoming the opposition leader quite recently, it seems that positive opinions are more common for him, unlike for Putin, and negative opinions are also less impactful.

![image](https://user-images.githubusercontent.com/90958123/156226506-1a9f4305-959e-427d-8f76-53c12cab1490.png)![image](https://user-images.githubusercontent.com/90958123/156226525-6d1b29d1-5458-42f4-9aa2-dde8d9d0f768.png)


  
Fig. 4. Pie charts of sentiments.


<b>Network analysis</b>

For network analysis I used NetworkX, package for the creation, manipulation, and study of the structure, dynamics, and functions of complex networks. I searched for co-occurrence in the cleaned previously tweets.

The network analysis of #Navalny and #Putin are shown on fig. 4 and fig. 5 respectively. 

![image](https://user-images.githubusercontent.com/90958123/156226620-7c0e74c1-6a8a-47e5-83ce-988bd7541e55.png)

 
Fig. 5. Co-occurrence of #Navalny,

 ![image](https://user-images.githubusercontent.com/90958123/156226632-00169676-0c79-455e-b322-a04f89ef68f2.png)


Fig. 6. Co-occurrence of #Putin.


<b>Conclusion</b>

The data and network analysis were performed. Several assumptions were confirmed. 

The bottleneck faced:

•	Twint does not detect language of the tweet (it is an actual bug), so we need to keep that in mind and filter later by language

Overall, we can see the notion of positive view of Alexei Navalny by twitter users. The most associated words with him are:

•	Sakharov prize (Alexei Navalny awarded the European Parliament’s 2021 Sakharov Prize)

•	Opposition

•	Jailed (Navalny was sentenced to 3 years for violating probation in a 2014 embezzlement case)

•	Kremlin critic

•	Democracy

•	Activism

The most associated words with Putin are:

•	Gender crime (Vladimir Putin has claimed the teaching of gender fluidity is a "crime against humanity")

•	Elections (in September election were held in Russia)

•	Gas (European gas prices have dropped after a meeting between Vladimir Putin and Gazprom officials)

•	Trump

In conclusion, people seem to grow warmer and warmer to a new opposition leader. As a person from Russia, I would say in significant way, because we tend to not have a very strong opinion on our political leaders.  
