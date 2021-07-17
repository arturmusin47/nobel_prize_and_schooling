### Hypo VS Alternative



## EDA
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




Considering Residence found that residence country is the same as birth_country for 5 records
nobel_science_df[['fullName','birth_country','birth_countryNow','death_country','death_countryNow','residence_1','residence_2','ind_or_org','country_of_affiliation_1','country_of_affiliation_2','country_of_affiliation_3','country_of_affiliation_4']][nobel_science_df.residence_1.notnull()]


Considering that we have to types of Birth Countries (original_old name and current_new name) in Nobel data set
and considering both types of the name in a separate stats (Example we have USSR and Russia) so decided to use field Birth Country (at the time of event)
Assuming that schooling data might be different from prev country name from new country so those will be treated as totally separate courty objects

Also Death Country is not used due to no real relationships from scholling perspective 


## Do all categories 



## Do only pure science categories # nobel_prize_and_schooling
