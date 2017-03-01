# Exploring-Gun-Deaths-In-The-US
Exploring the crime rate and killings in the United States based on various criteria from 2012 to 2014

- We read in the guns.csv file that contains the different attributes of killing like race, age, sex, place, educational background, intent, hispanic origin.
- Then we remove the header from the list of lists to clean the file and make it apt for analysis. 
- We count the gun deaths by year, months per year, race and sex.
- We read in a second dataset called census which gives us the total population based on each race. Using this data we compute the rate of gun deaths per race. 
- In order to get the raw counts of gun deaths per 100000 people in each race, we divide the total number of gun deaths by the population of each race. 
- We first map the races from each dataset as they have different naming conventions. After consolidating the data together we get the total population of each race. Using this data we filter out the killings based on intent - 'Homicide', Suicide', 'Accidental', 'Other reason'. 
- we iterate the race against the intent (eg: 'Homicide'), when the intent matches the keyword, the count of races are stored in a new dictionary. Then we calculate the total deaths using the total population per race and multiply that with 100000 to calculate the killings for each race every 100k people.
- We subsequently compute the gun death correlation to location and education, rate of intents by gender and race and exploring homicide rate by gender. 
