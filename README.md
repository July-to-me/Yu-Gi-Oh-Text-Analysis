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
- 


## Dataset

This dataset contains 12532 rows and 18 columns for the variables listed below. The following contains stats in Pokemon: A Pokemon has a unique set of stats that contribute to the Pokemon's identity. 

Variable  |Description |
-----|-----|
ID|The identification of the card|
Name|The card's name |
Type| If it is either a spell, trap, or monster card |
FrameType| Which variant of type it is (ex. if it is a monster type, is it an effect and synchro, or a normal, etc etc.) |
Desc|The description of what the card does or its text in the card.
Race| What type of subset the card is (ex. if a monster card is a warrior or dragon, or if a spell card is a continuous/quick-play spell card, etc etc.)
Archetype|The type of roster the card belongs to. A set of cards that work together for a common goal/playstyle. 
Atk|The attack points of a monster
Def |The defense points of a monster 
Legendary|This is a True/False statement that says if a Pokemon is a legendary Pokemon or not. 
Level|The stars on top of a monster, indicating 
Attribute|Similarly to race, it shows what subset the monster belongs to in terms of earth, water, dark, light, etc.
Scale |The pendulum monster's unique mechanic to special summon a set of monsters in the field if it meets the requirements.
Linkval|The link monster's unique summoning mechanic enables each link monster to use itself as material for other link monsters (non-link monsters can be considered as link 1 material unless stated otherwise).
Linkmarkers|Where the monster's link arrows point to.
Banlist_info|To show wether a card is not playable or not. To also show how many copies can one person be able to run in a legal tournament.

