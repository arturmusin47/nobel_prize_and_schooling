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
    
    
### Data Visualization

<img src="Number of Nobel winners by country in pure science categories.png" >
<img src="Top 20 Countries with Nobel winners in pure science.png" >
<img src="Average age of Nobel winners in pure science.png" >
<img src="Correlation between schooling and winners USA.png" >
<img src="Correlation between schooling and winners UK.png" >



### Statistical Inference
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
2. It's been discovered that there is no direct correlation between schooling years and number of nobel winners considering the rise of shooling years for USA and UK within the period of time when people are schooled in those countries. 


Considering Birth_country and Death_country found that Death_country doesn't play a role in our main question  by below 2 examples 
so excluding Death_country

Abdus Salam
https://en.wikipedia.org/wiki/Abdus_Salam#Youth_and_education
Wolfgang Pauli
https://en.wikipedia.org/wiki/Wolfgang_Pauli

Abhijit Banerjee
https://en.wikipedia.org/wiki/Abhijit_Banerjee

Riccardo Giacconi
https://en.wikipedia.org/wiki/Riccardo_Giacconi
Giacconi received his Laurea from the Physics Department of University of Milan 

Carlo Rubbia
https://en.wikipedia.org/wiki/Carlo_Rubbia


Richard Adolf Zsigmondy
https://en.wikipedia.org/wiki/Richard_Adolf_Zsigmondy

John Macleod
https://en.wikipedia.org/wiki/John_Macleod_(physiologist)


Georg von Békésy -- DID NOT GO TO SHOOL WHERE HE BORN
https://en.wikipedia.org/wiki/Georg_von_B%C3%A9k%C3%A9sy

Tadeusz Reichstein -- DID NOT GO TO SHOOL WHERE HE BORN
https://en.wikipedia.org/wiki/Tadeusz_Reichstein

Polykarp Kusch -- DID NOT GO TO SHOOL WHERE HE BORN
https://en.wikipedia.org/wiki/Polykarp_Kusch

Considering Residence found that residence country is the same as birth_country for 5 records
nobel_science_df[['fullName','birth_country','birth_countryNow','death_country','death_countryNow','residence_1','residence_2','ind_or_org','country_of_affiliation_1','country_of_affiliation_2','country_of_affiliation_3','country_of_affiliation_4']][nobel_science_df.residence_1.notnull()]


Considering that we have to types of Birth Countries (original_old name and current_new name) in Nobel data set
and considering both types of the name in a separate stats (Example we have USSR and Russia) so decided to use field Birth Country (at the time of event)
Assuming that schooling data might be different from prev country name from new country so those will be treated as totally separate courty objects

Also Death Country is not used due to no real relationships from scholling perspective 


## Do all categories 



## Do only pure science categories # nobel_prize_and_schooling












Install help:
pip install -U --no-deps mapclassify git+git://github.com/geopandas/geopandas.git@master
pip install git+git://github.com/geopandas/geopandas.git






## Data Source 
Websites and/or databases (linked here): 
https://www.kaggle.com/imdevskp/nobel-prize
https://ourworldindata.org/grapher/correlation-between-mean-years-of-schooling-and-gdp-per-capita
