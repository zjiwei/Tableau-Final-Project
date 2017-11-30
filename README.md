# Tableau-Final-Project

As graduate students, we are all looking to improve our current employment status. This could involve changing positions within our current companies, getting a job at a new company within our current field, or completely switching industries. While finding a job can be an incredibly stressful experience, many students have the additional challenge of obtaining an H1B visa to work in the United States. Members of our group, as well as many of our fellow masters students, may one day need to obtain a visa to stay in the United States; making this analysis personally useful.

Regardless of our eventual employment status, it will be helpful for every member of the group to learn about who is getting hired, where they are employed, and what salaries they are being paid. We will be able to see where people with similar master's degrees are getting hired and the success rate of applications in various locations around the United States.

Lastly, our group wanted to seek out a robust data set that we could practice our newly developed skills on. Our selected data set contains over 3 million records of H1B visa applications, containing a variety of data types from binary (acceptance status), numerical (salary), and location data (location of employer) to provide a wide range of possible analyses we can perform. 

Our dataset contains information about H1B visa applicants. In our analysis, we aim to identify the features of H1B visa applicants, their potential employers, and their offered salaries. From this data, we can acquire a grasp of where potential H1B visa applicants have better chances of employment.

Getting familiar with the software Tableau appeared to be very beneficial in handling and analyzing our data.  Tableau offers a lot of features which enabled us to clean our data. For instance, using Data Interpreter, we were able to delete null or missing values for each variable. In Tableau, we got familiar with Sheets in which we can create different visualizations of different dimensions of our dataset with different measures. For instance, we chose prevailing wage and case status to see if there exists a potential relation between these two variables. We observed that the average prevailing wage for those, whose H1B visa got certified is $72,767, while this figure is much larger for the denied cases, for which the average prevailing wage was recorded as $2,245,191.

![Wage~Case](https://github.com/zjiwei/Tableau-Final-Project/blob/master/Wage~CaseStatus.PNG)

The Show Me option, on the top right corner of our Sheet window,  recommends what kinds of charts or graphs can be used as visualization tools, based on the features of our dataset.

The following chart is a very useful illustration of the relation between certified cases with Full-time or Part-time status and average prevailing wage.

![Wage~Case~FullTime](https://github.com/zjiwei/Tableau-Final-Project/blob/master/Wage~CaseStatus~FullTime.PNG)

We also learned how to manage metadata by creating hierarchy of folders, changing data types and creating calculated fields. Our data can be saved and published and will still keep its interactive feature. 

We were able to use Tableau to detect the presence of large outliers in the data. For the variable Prevailing Wage, using the Create Groups function, we found that a record had a value of almost 7 billion dollars. Many other applications had prevailing wage values in the hundreds of millions (see figure below). For our analysis, we may want to exclude these records, since our goal is to help MSBA students understand the dynamics behind the visa process in the US, and that we probably won’t be applying to jobs making over a billion dollars per year after the program.

![Filter](https://github.com/zjiwei/Tableau-Final-Project/blob/master/Filter.png)

Tableau is extremely useful in both data processing and data visualization. For example, there is information about worksites in our dataset but each row contains both cities and states. Using Tableau, we can use custom split to divide them into cities and states which will play a key role in our further analysis. In Tableau, it is easy to change our data into types, including the extremely useful geographical, according to our needs. 

We are able to take a textual field like “worksite” and modify it into both City and State Worksite fields.Using these new fields, we can start to learn about the geographical characteristics of applicants.

![Location~H1B](https://github.com/zjiwei/Tableau-Final-Project/blob/master/Location~H1B.PNG)

We identified location as an important factor to investigate because job hunting in locations where H1B Visa applicants have had previous success could indicate an area where their skills are more in demand. Tableau provides visualization methods that are useful and extremely easy to implement. We can use symbol maps to show the information more directly. According to the graph above, we can know there a number of opportunities in the state of California, New York, and Texas. 

![Location~H1B~Wage](https://github.com/zjiwei/Tableau-Final-Project/blob/master/Location~H1B~Wage.PNG)

In addition to where H1B applicants are most likely to get jobs, we would like to investigate the average wage of certified applicants in different states. The graph above shows there is little difference in wage in most states and the highest average wage is located in the state of New Mexico.
Our dataset also provides information about job types, so it is possible to analyze the number of applicants in different jobs. Surprisingly, the jobs of most applicants are related to computer or software.

![H1B~Soc%20Name](https://github.com/zjiwei/Tableau-Final-Project/blob/master/H1B~Soc%20Name.PNG)

Focusing on the certified group and including the data of wage, we can know that there is great difference in different types of jobs. Thanks to the interactive interface in Tableau, we are able to know details of each point.

![CWS](https://github.com/zjiwei/Tableau-Final-Project/blob/master/CWS.PNG)

