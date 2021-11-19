# Hip Hop Lyrics Capstone Project
## Using Data Modeling to predict the Hip Hop Artist from Lyrics -  Tab Chapman

### Description
---
As Hip hop cements its position as the popular genre of music in the United States , it is important to understand the forces that propelled it from relatively obscure beginnings in the Bronx to world status. One of these forces is lyrics. Past studies have found that Hip Hop songs have more lyrical variety and larger vocabulary than other popular genres such as Rock or Pop. One element of lyricism that is different from other forms of popular music is the element of personal voice in the lyrics. Hip Hop lyrics are almost always written by the artist performing the song or at least written from the artist's perspective. The goal of this project is to build a model that predicts the given artist given the lyrics to better understand the lyricism of different artists. 


### Web Scrapping
---
Lyric data was scraped from Genius API using the python wrapper LyricsGenius. I decided to use the top ten most popular songs from the top fitly artist due to time and memory constraints. To get info on artist popularity I scraped web data from billboard. 


### Modeling
---
Neural Nets, Ada Booost and Random Forest were used. Random Ferest had the best results at 0.35 testing accuracy.

### Text Generation 
---
A fake song was created with just Playboi Carti lyrics with Markovify. Urberduck was used to fake the voice.




### Software Requirements
---
Web scraping: requests, lxml, beautiful soup and pandas, 
Modeling: pandas, tensorflow, keras, matplotlib, sklearn, and numpy
Text Generation: Markovify

Uberduck:https://uberduck.ai/#voice=playboicarti&mode=tts-basic



### Dictionaries
---
**Code Dictionary:**

|File Name|Folder|Description|
|---|---|---|
|Scrapping|code|Notebook for web scraping lyrics| 
|EDA|code|Notebook for permorming EDA and data cleaning|
|Modeling|code|Notebook for modeling and predicting|



**Dataset Dictionary:**

|Folder Name|Description|
|---|---|
|Carti_text|Carti Text for Markov|
|Clean_lyrics|clean lyrics for EDA|
|English|list of explatives in english|
|Lyrics_all_1|transformed lyrics|
|Lyrics_corpus|lyrics in text format for Markov|
|lyrics|Raw Lyrics|