# Business Understanding
## Overview
The company is expanding into new industries to diversify its portfolio. The company has plans to purchase and operate aicrafts for both commercial and private use. The  company is expandingin to new industries to diversify its portfolio. Specifically, they are interested in purchasing and operating aircrafts for commercial and private enterprises but do not know anything about the potential risks of aircraft. You are charged with determining which aircraft are the lowest risk for the company to start this new business endeavor. You must then translate your findings into actionable insights that the head of the new aviation division can use to help decide which aircraft to purchase.

# Business problem
The biggest risk in the aviation industry is safety which might result to serious damages to a business and even more  for a new venture. The above may lead to brand damage and heavy financial implications. 

- To determine the relationship between flight category(private,commercial) and the extent of injuries.
- To determine the relationship between flight category(private,commercial) and the extent of injuries.
-  Determine the relationshop between flight category(private, commercial) and the extent of injuries.
-  Provide three actionable recommendations for aircraft investment decisions

Why : Conducting a risk assessment analysis enables the company to understand risks associated with different aircrafts. This will ensure reduced accident occurence,safer operations, and maximization of investments in the aircraft venture.

## **Stakeholders**
- Company Executives-people who needs insights before purchasing the flights
- Operations team for the company-team that will be handling the aircrafts

Key columns to be used are: Make,Model, Flight.Category, Total.Fatal.Injuries, Total.Minor. Injuries, Total. Serious.Injuries, and Engine.Type


#### Overview
After understanding our dataset, we will now take subsequent steps to be able to handle our data **Data Preparation**.
This will involve cleaning our data, formatting some rows as we prepare our data for analysis.

The main goals of this step are to:
1. Handle duplicates in our data  
2. Identify and handle missing values in our data  
3. Fix data types 
4. Identify columns to be used 
5. Create new columns for risk analysis
5. Ensuring data is ready for data analysis and visualization

## Data Understanding & Analysis
The data IS from the National Transportation Safety Board that includes aviation accident data from 1962 to 2023 about civil aviation accidents and selected incidents in the United States and international waters. From the data, we see that there has been a significant drop in numbers of injuries over time. This may be due to the newer generations of aircrafts being used which use the katest technologies.


From the data, From the data, we see that there has been a significant drop in numbers of injuries or accidents over time. This may be due to the newer generations of aircrafts being used which use the latest technologies in aviation.

For someone who wants to venture into this line of business, making safety their competitive advantage will be an added advantage
<img width="3354" height="171" alt="image" src="https://github.com/user-attachments/assets/33fa2891-1d71-4f98-b50c-3892cf895785" />

## Description of data.
After the data was loaded, it contained 90,348 rows and 31 columns. After the data was cleaned, removing duplicates the rows dropped to 88,958 rows and 21 columns that were used in the analysis.

For the categorical columns, some data had whitespaces and place holders which were removed to fully standardize the data. 

Columns which had a very high number of null values were dropped, an the remaining were filled with Unknown. The Nan values were deliberately kept to offer insights in terms of the data being analyzed.

For numerical columns, issing values were filled with medianbecause it preserves the distribution and does not distort analysis.

For column such as Purpose of flight, the column was split using mapping and a new column name created called flight categort(private and commercial planes)

The objective here is to calculate risk metrics and produce clear recommendations to support business recommendation for our client.
To meet the business goals, data was majorly analyzed using groupby method. 
- Grouping injuries by Flight.Category to compare injury severity.
- Analyzing correlation between No of engines with aircraft damage

We will be able to create multiple views on:
1. To determine the relationship between flight category (private,commercial) and the extent of injuries.
2. To analyze the relationship between aircraft make and model with injuries.
3. To analyze aircraft damage in relation to engine type and no of engines.

## Visualizations

Insight Findings
#### Key Findings
Flight category compared with injuries and fatalities

- From our analysis, private planes reported the highest numbers of injuries overally with 21,523 fatal,12,387 serious and 15,277 minor. 
Interpratation-private plates exprinece significant more fatalities and injuries maybe due to their size, less rigorous maintenance and maybe inexperienced pilots.

- Unknown category-23,062 fatal injuries, and also has the highest fatal count.
Interpration: Since the data has alot of unclassifies and unreported flights, there might be incomplere data to conclusively interptrate this.

- Commercial categories
From the analysis, commrcial aircrafts reported the lowest number of injuries with 5616 fatal,3036 serious and 3,776 minor.
- Interpratation- Commercial flights have the best safety records due to stict safety regulations, experienced crews and advanced aircraft technologies.

- Therefore based on this, private aircrafts show most injuies across all categories, making them a riskkier for business operations. Comercial aircrafts remain the safest option wuth lowest fatalities and injuries. It will be prudent to advise the client to base his enterprise more on commercial planes than private planes. Commercial planes are the better safer option and also reliable.

  #### Conclusion-Make
- From the analysis, the top 10 aircrafts with the highest number of falaties are cessna, boeing, piper , beech etc have the highest number of fatalities. If we fully  depended on this data to advise the client, then we would recommend other crafts that do not have hifg record of fatalities for this business.
- Comparing the aircraft make, might help us decide on which model to purchase depending on how many accidents they are involved in.

- #### Conclusion-Engine Type Vs Damage
- Single engine aircraft(1 engine) have the highest proporton of substantial damage of about 75%.
- They are closely folowed by destroyes at 20% and only a small proprportion of minor or unknown damage.
Interpratation- Single engine planes are more vulnerable to substantial or complte damage in accidents.

- Two engines-Substantial dama(53%),Destroyed(25%), minor(10%) and unknown(11%).  Two engine are failrly better than single engines.
- Aircrafts with 6 and eight engines, their substantial damage is rare and small for 6-enginse and 67% for 8-engine.

Overal insights. 
- Substantial damage are common in all engine types.
Planes with (3-4) engines appear to reduce the proportion of severe outcomes maybe fue to better safety features.
- Single engine are the most risk in terms of damage.


#### Recommendations
- Based on the analysis, it is advisable for the client to invest primarily in commercial aircrafts. They are proven and demonstrate to be superior, safer, reliable. Private planes though common have higher accidents and may require stricter maintenance and qualifies human resource.

- Preference should also be given to planes with multiple engines and turbo-powered models with proven safety records.
  
- Avoid aircrafts with consistently high accident records and prioritize those that demonstrate safety.

- Engine type is a key factor. Commercial grade engines demonstrate better durability and lower destruction rates as compared to those in small private aircrafts.

- Companies should purchase aircrafts with more than three engines as they have a reduces proportion of severe aircraft damage.

- Commercial flights have the best safety records due to strict safety regulations, experienced crews and advanced aircraft technologies.


  #### Tools used
  - Python(Pandas, Matplotlib,Seaborn)
  - -Tableau for dashboard vsualization
  - GitHub
  - Jupyter Notebook for data analysis
    
  #### References
  -National Transportation Safety Board(NTSB)
  -Federal Aviation Administration(FAA) Accidents Statistics 2023.

