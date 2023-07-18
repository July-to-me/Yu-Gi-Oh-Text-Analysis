# Yu-Gi-Oh-Text-Analysis
The objective of this  project is to demonstrate my data-slicing skills, as well as cleaning. I also wanted to see any trends that go on with various card types, since it is common for the Yu-Gi-Oh! The community thinks that there has been an increase in card text. I want to use R packages such as quanteda, tidytext, and wordcloud.


## Objective

In this project, I wanted to see if I can predict how many statistical analyses can I do in this dataset since I am a huge fan of playing the trading card game to this day:
1. Getting the data via ygoprodeck, and loading it in PostIt.
3. Creating various data frames in order to group them based on monster, spell, and trap types to do Exploratory Data Analysis.
4. I then used statistical techniques such as ANOVA, K-Means clustering, and others to answer my questions about general card text trends.
5. I later used different machine-learning techniques to predict how long card text will get as time goes on, or the distribution of each card type.

## Dataset

I've used a dataset that I found on ygoprodeck.com. This is a website that has all the cards and their text given in a JSON text format. This is extremely nice since I am able to get the card text as quickly and efficiently as possible. 

More info about the JSON and database can be found here:
- Website: https://ygoprodeck.com/card-database/?&num=24&offset=0

## Discovery

Here is a small conclusion that I've found based on my findings:
- Pokemon with one type from generation 5-7 has experienced a big nose dive in representation. We can also see Pokemon with two types did also suffer from not having a lot of representation as well.
- Overall, the population between one-type and two-type Pokemon does seem similar until the mentioned nose dive from generation 5-6, where two-type Pokemon have more representation in Pokemon games.
- When conducting a T-test, I found that Pokemon with two-type and one-type are statistically significant from one another. This means that Pokemon with two types, on average, had usually higher stats than pokemon with one type.
- Water types have a big representation at a whopping 10.63%, followed by Normal-types 9.40%. But when it comes to legendary Pokemon, Psychic, and Dragon-types become the most potent (16.84% and 11.05% respectively).
- Shockingly Fire types are not even the top 5 most frequent types despite being the main 3 types to be selected at the beginning of the game as a starter Pokemon. As well as not being a potent type when it comes to legendary Pokemon.
- Every 'Total' stat, on average (per generation/region), for non-legendary-pokemon has been very consistent.
- Same goes for legendary but generation 7th (Alola) has experienced an average total stat of 561 (a huge 10% decrease of the total average of all legendaries)
- Thanks to ANOVA, we now know that a lot of types do contain stats that are statistically significant from one another.
- The Attack stat/attribute for all Pokemon was statistically significant, based on regions/generations. (I assume it is because of the outliers of the different regions/generations)
- We can also see that HP and Defense were the ones that were most statistically significant across different regions(based individually per type).
- Ghost-types have a random distribution of stats than other typings. This means that there may be no way of predicting where what stat/attribute will be more prominent in the next set of generations.


## Dataset

This dataset contains X rows and Y columns for the variables listed below. The following contains stats in Pokemon: A Pokemon has a unique set of stats that contribute to the Pokemon's identity. 

Variable  |Description |
-----|-----|
Total|The accumulation of all the stats below|
HP|Also known as "Hit Points": The Health of the Pokemon |
Attack|The physical attack strength of the Pokemon |
Special Attack|The non-physical attack moves from the Pokemon |
Defense|How much can a Pokemon withstand physical attacks
SpecialDefense|How much can a Pokemon withstand non-physical attacks
Speed|This dictates which Pokemon can attack first
Generation|Where the Pokemon is from. Generation and Region will be used interchangeably.
Type 1 and Type 2 |This is the attribute of the Pokemon. There are 18 types in the world of Pokemon. A Pokemon can have just one typing or two. 
Legendary|This is a True/False statement that says if a Pokemon is a legendary Pokemon or not. 
