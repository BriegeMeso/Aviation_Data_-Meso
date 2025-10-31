Overview
# Overview
The company is expanding into new industries to diversify its portfolio. The company has plans to purchase and operate aicrafts for both commercial and private use. Your company is expanding in to new industries to diversify its portfolio. Specifically, they are interested in purchasing and operating airplanes for commercial and private enterprises, but do not know anything about the potential risks of aircraft. You are charged with determining which aircraft are the lowest risk for the company to start this new business endeavor. You must then translate your findings into actionable insights that the head of the new aviation division can use to help decide which aircraft to purchase.

Business Understanding
# Business problem
The biggest risk in the aviation industry is safety which might result to serious damages to a business and even more  for a new venture. The above may lead to brand damage and heavy financial implications. 

- To determine the relationship between flight category(private,commercial) and the extent of injuries.
- To determine the relationship between flight category(private,commercial) and the extent of injuries.
-  Determine the relationshop between flight category(private, commercial) and the extent of injuries.
-  Provide three actionable recommendations for aircraft investment decisions

Why : Conducting a risk assessment analysis enables the company to understand risks associated with different aircrafts. This will ensure reduced accident occurence,safer operations, and maximization of investments in the aircraft venture.

## **Stakeholders**
- ** Company Executives-people who needs insights before purchasing the flights
- ** Operations team for the company-team that will be handling the aircrafts

  
Data Understanding
The data usied is from Aviation_Data_csv. The data has 90398 entries.
Key columns to be used are: Make,Model, Flight.Category, Total.Fatal.Injuries, Total.Minor. Injuries, Total. Serious.Injuries, and Engine.Type


#### Overview
After understanding our dataset, we will not take subsequent steps to be able to handle our data **Data Preparation**.
This will involve cleaning our data, formatting some rows as we prepare our data for analysis.

The main goals of this step are to:
1. Handle duplicates in our data  
2. Identify and handle missing values in our data  
3. Fix data types 
4. Identify columns to be used 
5. Create new columns for risk analysis
5. Ensuring data is ready for data analysis and visualization

## DATA Analysis & Visualization
The objective here is to calculate risk metrics and produce clear recommendationst to support business recommendation for our client.

To meet the business goals, data was majorly analyzed using groupby method. \
- Grouping injuries by Flight.Category to compare injury severity.
- Analyzing correlation between No of engines with aircraft damage

We will be able to create multiple views on:
1. To determine the relationship between flight category (private,commercial) and the extent of injuries.
2. To analyze the relationship between aircraft make and model with injuries.
3. To analyze aircraft damage in relation to engine type and no of engines.

   
Insight Findings
#### Conclusion-Flight category

- From our analysis, private planes reported the highest numbers of injuries overally with 21,523 fatal,12,387 serious and 15,277 minor. 
Interpratation-private plates exprinece significant more fatalities and injuries maybe due to their size, less rigorous maintenance and maybe inexperienced pilots.

- Unknown category-23,062 fatal injuries, and also has the highest fatal count.
Interpration: Since the data has alot of unclassifies and unreported flights, there might be incomplere data to conclusively interptrate this.

- Commercial categories
From the analysis, they have reported the lowest number of injuries with 5616 fatal,3036 serious and 3776 minor.
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

  #### Tools used
  - Python(Pandas, Matplotlib,Seaborn)
  - -Tableau for dashboard vsualization
  - GitHub
  - Jupyter Notebook for data analysis
    
  #### References
  -National Transportation Safety Board(NTSB)
  -Federal Aviation Administration(FAA) Accidents Statistics 2023.

