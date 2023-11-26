Project 4 - Tableau

Overview
The aim of this project is to analyse and visualize information from a specific dataset and/or any other source by using Tableau. 

Requirements/Libraries used:
- Pandas
- BeautifulSoup
- Requests
- Re
- Time

Methodology
I have chosen a dataset from Kaggle called "World Educational Data" (updated 18 days ago). I have done Exploratory Data Analysis on it and found many relevant variables to work on. I immediately thought I could focus on the difference of OORS (out-of-school rate) between men and women in the different educational levels, the relation between education and birth rate, and the relation between education and the unemployment rate. I also thought it would be interesting to see if there is difference among countries. 
Besides, I wanted to check if countries with the best universities corresponded to any of these variables. Therefore, I did web-scraping on https://cwur.org/2021-22.php to obtain the countries of the universities included in the list of "World University Rankings 2023". 

I have done some queries in SQL to obtain the information I wanted to create the plots.

Link to my story:
https://public.tableau.com/app/profile/martina.rivero/viz/Tableau_Project_17004254847260/GlobalEducation?publish=yes

In Tableau, I imported both datasets and made a left join to have the full information of the first dataset and add the information of the countries with the most important universities. I started by plotting the differences between male and female in OORS in the different educational levels in all countries which had at least one datapoint. It was very difficult to visualize because of the number of countries, so I filtered considering the countries with the highest numbers. This way, I could better visualize the plot. 

I was also curious about maths and reading skills. Analysing these skills is a way of understanding how good a country is in educational terms. A map was the perfect fit to visualise both variables. Many countries are in the lightest shade of colour because there is no information to display. Even though the dataset is pretty complete, still there is some missing information. It could be that governments do not collect this information or that they do not want to share it. 

Next, I wanted to check if there was any correlation between the maths and reading skills and the unemployment rate and the birth rate. In order to visualize it, I used scatter plots in which each point in the plot is a country. I decided to do different plots to understand the correlation between each variable:
First one compares maths proficiency to unemployment rate
Second one compares reading proficiency to unemployment rate.
Third one compares maths proficiency to birth rate.
Fourth one compares reading proficiency to birth rate.  

Afterwards, I chose a treemap to see if there was any correlation between the countries with the top universities and the birth and unemployment rates. I found this type of plot interesting as it shows information in an easy way. The size of the squares corresponds to the number of world top universities in that country. The number in each square indicates the birth rate and the unemployment rate in each country. The shade of the colour correspond to the birth rate and the unemployment rate in each of the plots.

Having the information of world top universities and the upper secondary completion rate, I thought it was going to be compelling to analyse if there was any relationship between them. Thus, I chose packed bubbles with the size depending on the number of top universities and the colour depending on the upper secondary completion rate. I used the same plot to compare top universities to maths & reading skills. In this case, the shading purple colours correspond to the level of the skills. As darker as it becomes, the better the country is in these skills. The maths & reading skills is a variable defined as a simple sum of the maths skills and the reading skills.

After having all these plots, it was necessary to create dashboards that could relate different plots and a story that could unify all the dashboards and have it in a way that could be exposed to an audience. 

- In the first two pages, the aim of the study is described: 
  Analyse and understand variables related to education in a worldwide perspective and check if they are related between them and if they have an impact on birth rate and/or unemployment rate. 
- Page "OOSR" describes the difference between men and women out-of-school rate. In other words, it checks if gender is an important factor for leaving education from pre-primary up to secondary levels. 
- Page "Maths & Reading Skills" shows how these skills can be different depending on the country. Besides, it shows the relationship between the countries where the world top universities are located and the how good those countries are in maths and reading. 
- Page "Skills vs Unemployment Rate" identifies the correlation between each of the skills and the unemployment rate. Same analysis is done in the following page "Skills vs Birth Rate" but identifying the correlation between these skills and birth rate. 
- Page "Top Universities" checks if there is any correlation between the countries with the top universities and the birth and unemployment rate. Furthermore, it tests if these countries coincide with the ones with a high upper secondary completion rate. 
- Last page defines the conclusions of the study. 

Conclusions
In general terms, there is no such a big difference between male and female OOSR. Although in cases where there is a difference, female OOSR is higher compared to male OOSR. Abandoning school happens more in pre-primary and upper secondary educational levels. It can also be detected that the countries with more OOSR are third world countries. There are some countries that are repeated in more than one plot, i.e. Syria, meaning that they have a very high OOSR, no matter the educational level. It would be interesting to study if there is any pattern that covers all of these countries and that could explain this high OOSR. For instance, war could be one of the causes for a high OOSR, like in Syria. 

Regarding skills, it is necessary to consider that they are considered for students between 2nd and 3rd grade (8-9 years old). In general, where there are good maths skills, there are also good reading skills. The maps shows how these skills are related and probably it is because the educational level is either generalised good, neutral or generalised bad. Anyway, It can be said that worldwide, reading skills are better than maths skills. There are some countries that do not have information with respect to these variables. That is why it surprising that USA, France or Germany have such a clear colour. It would be ideal to standardise the method of acquiring information so that working with world educational data could be easier. 

The packed bubbles called "Top Universities vs Math & Reading Skills" includes only the countries with information of skills. There is no a precisely direct relationship between countries with top universities and great skills but still there is a relationship. Some of the big bubbles are painted with a dark purple meaning that their domain of skills is very good at primary levels. There are some other medium bubbles with a clearer purple like India, Brazil, Iran and Mexico, which means they have many top universities but their maths & reading skills are not so good compared to other countries. 

When analysing the skills vs the unemployment rate separately (math proficiency separate from reading proficiency), an important difference is noticed. In maths, the datapoins are more disperse, but in general terms, as higher the math proficiency, as lower the unemployment rate. It can be affirmed that the maths skills have a direct impact on the unemployment rate. As expected, Japan, Singapore and Norway are the countries with one of the highest math proficiency and one of the lowest unemployment rate. Surprisingly, Uruguay is better than Spain in both aspects. Maths skill is higher and the unemployment rate is lower. 

On the contrary, there is no correlation between the reading proficiency and the unemployment rate. The data points are even more disperse than in the previous plot. Therefore, reading skills do not have a direct impact on the unemployment rate. Again, Norway and Singapore are one of the countries with the best reading skills and the lowest unemployment rate. In the comparison of these variables, Uruguay is still better than Spain because although Spain is better at reading skills, the difference between the unemployment rate is still high. 

When analysing the same skills against the birth rate, the relation is much more direct. Data points are less disperse and there is a pattern of a line with an ascending scope. Where both maths & reading skills are high, the birth rate is low. Undoubtedly, Japan, Singapore and Norway are the countries with the best situations. In this relations, Spain is better located compared to Uruguay because the birth rate is lower. It can be concluded that the maths & reading skills have an influence on the birth rate. This would be a next step to be studied. It could be because women are not studying and thus have more time or less family planning and get pregnant with more frequence. 

At the moment of checking the countries with the best universities in the treemaps, as it could be expected, USA is number 1. China and Japan are the followers. Spain is also one of the most important ones. If these countries are compared to the birth rate, it can be visualised that there is no relation between them. The colours of the squares does not follow a pattern. The shades are very different in different parts of the treemap. However, top countries are not painted with dark blue, which means that although there is not a direct relation, countries with top universities have a lower birth rate compared to other countries. 
For the unemployment rate, the conclusion is similar. There is no a direct correlation. It looks as if squares were painted randomly. USA has a high unemployment rate! Spain too! In other words, having world top universities will not influence the birth and unemployment rates. 

Last but not least, it was interesting to see if countries with the top universities coincided with the ones with the highest upper secondary completion rate. First, it must be mentioned that USA, Japan, United Kingdom, France, Germany, Italy, South Korea are not taken into account because there is no "upper secondary completion rate" available for them. Regarding the ones that do have information, the conclusion is that there seems to be a relation (not strictly direct) between countries with top universities and upper secondary completion rate. China, Brazil and Chile have a pretty dark blue colour. For the small circles, the colour becomes a clear sky-blue. 

All in all,

- Small difference between female OOSR and male OOSR. 
- Where there are good maths skills, there are good reading skills. 
- Countries with top universities may possibly have great skills.
- As higher the maths proficiency, the lower the unemployment rate. 
- Previous sentence not applicable to reading proficiency. 
- As higher the skills, the lower the birth rate is. 
- No specific relation between top universities and rate birth.
- No specific relation between top universities and unemployment rate. 
- Top universities countries probably have a high upper secondary completion rate.
