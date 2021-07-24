### Background and Motivation


Purpose of the project to find out correlation between Nobel Prize Winners in pure science categories in pure science categories and number of schooling years by counrty.

Alfred Nobel was a Swedish chemist, engineer, and industrialist most famously known for the invention of dynamite. 
The Nobel Prize is five separate prizes that, according to Alfred Nobel's will of 1895, are awarded to ”those who, during the preceding year, have conferred the greatest benefit to humankind.
Nobel Prizes are widely regarded as the most prestigious awards available in their respective fields
Schooling years average number of years of total schooling across all education levels for the population.
https://en.wikipedia.org/wiki/Nobel_Prize
http://piketty.pse.ens.fr/files/LeeLee2016.pdf



## Data Description
Datasets are in csv format with 46950 rows with 7 columns for first dataset and 950 rows with 52 columns for second dataset. 
Nobel prize dataset: the features of interest are Nobel Prize winner names and countries where each laureate related to. 
Schooling year dataset: the features of interest are Total years of schooling and Entity/Code (country)



### Hypo VS Alternative



## EDA
+ **Time period** (1817 - 1997)
+ **Groups** (Countries)
+ **Base** (Birth countries and Year of schooling start per winner)
+ **Provisions** (counts):
    + Total winners (excluding organizations)= 923
    + Total winners in pure scince = 700
    + Total winners in pure scince in USA = 246 
    + Total countries in Nobel prize dataset = 55
    + Total countries in schooling dataset = 293
    
    








### Statistical Inference and  Data Visualization
Observations and findings after EDA:

Pre-step. Out of 10 columns related to counrty-winner relation 'Birth Country' column selected as main feature from nobel data by simply running random selection of 20 winners and by manually checking if birth counrty and schooling country is the same. Only 3 out of 20 randomly selected winners born in one counrty and schooled in another counrty (85% confidence).

DID NOT GO TO SHOOL WHERE THEY BORN:
- Georg von Békésy
https://en.wikipedia.org/wiki/Georg_von_B%C3%A9k%C3%A9sy

- Tadeusz Reichstein
https://en.wikipedia.org/wiki/Tadeusz_Reichstein

- Polykarp Kusch
https://en.wikipedia.org/wiki/Polykarp_Kusch

1. Considering USA as leading counrty by winners by huge outperformance over the rest countries in the nobel prize winners dataset and United Kingdom being a second top countries. USA and UK selected for further analysis to find correlation between schooling years and number of nobel winners in science. 

<img src="Number of Nobel winners by country in pure science categories.png" >
<img src="Top 20 Countries with Nobel winners in pure science.png" >

2. Additionally observed average age of the winners which is 59 years where youngests are 25 and oldests laureates are 97. Interestingly winners ages are normally distributed.

<img src="Average age of Nobel winners in pure science.png" >

3.Coming back to a main qiestion it's been discovered that there is actually no direct correlation between schooling years and number of nobel winners considering the rise of shooling years for USA and UK within the period of time when people are schooled in those countries. 
Scholling years change and nobel winners follow a different distribution and do not correlate in USA and United Kingdom.


<img src="Correlation between schooling and winners USA.png" >
<img src="Correlation between schooling and winners UK.png" >



## Do all categories 



## Do only pure science categories # nobel_prize_and_schooling















## Install help:
pip install -U --no-deps mapclassify git+git://github.com/geopandas/geopandas.git@master
pip install git+git://github.com/geopandas/geopandas.git


## Data Source 
Websites and/or databases (linked here): 
https://www.kaggle.com/imdevskp/nobel-prize
https://ourworldindata.org/grapher/correlation-between-mean-years-of-schooling-and-gdp-per-capita
