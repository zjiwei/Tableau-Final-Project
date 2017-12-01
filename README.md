# Tableau-Final-Project

### Why Our Story is Important

As graduate students, we are all looking to improve our current employment status. This could involve changing positions within our current companies, getting a job at a new company within our current field, or completely switching industries. While finding a job can be an incredibly stressful experience, many students have the additional challenge of obtaining an H1B visa to work in the United States. Members of our group, as well as many of our fellow masters students, may one day need to obtain a visa to stay in the United States; making this analysis personally useful.

Regardless of our eventual employment status, it will be helpful for every member of the group to learn about who is getting hired, where they are employed, and what salaries they are being paid. We will be able to see where people with similar master's degrees are getting hired and the success rate of applications in various locations around the United States.


### About the Data

Our group wanted to seek out a robust data set that we could practice our newly developed skills on. Our selected data set contains over 3 million records of H1B visa applications, containing a variety of data types from binary (acceptance status), numerical (salary), and location data (location of employer) to provide a wide range of possible analyses we can perform. 

Our dataset contains information about H1B visa applicants. In our analysis, we aim to identify the features of H1B visa applicants, their potential employers, and their offered salaries. From this data, we can acquire a grasp of where potential H1B visa applicants have better chances of employment.


### Initial Analysis and Using Tableau

Getting familiar with the software Tableau appeared to be very beneficial in handling and analyzing our data. Tableau offers a lot of features which enabled us to clean our data. For instance, using Data Interpreter, we were able to delete null or missing values for each variable. In Tableau, we got familiar with Sheets in which we can create different visualizations of different dimensions of our dataset with different measures. For instance, as seen in Figure 1, we chose prevailing wage and case status to see if there exists a potential relationship between these two variables. We observed that the average prevailing wage for those, whose H1B visa got certified is $72,767, while this figure is much larger for the denied cases, for which the average prevailing wage was recorded as $2,245,191.

![Wage~Case](https://github.com/zjiwei/Tableau-Final-Project/blob/master/Wage~CaseStatus.PNG)

**Figure 1. Prevailing Wage by Case Status**

This number included major outliers, such as applications with prevailing wages over $6 billion. Even after excluding outliers, however (> $500,000), we still found that denied cases had much higher prevailing wages than other cases statuses.

![RelevantWage~CaseStatus](https://github.com/zjiwei/Tableau-Final-Project/blob/master/RelevantWage~CaseStatus.png)

**Figure 2. Relevant Wage by Case Status**

The Show Me option, on the top right corner of our Sheet window,  recommends what kinds of charts or graphs can be used as visualization tools, based on the features of our dataset.


### Part-time vs. Full Time

One question our group was interested in is the differences between full and part time jobs. We were interested in learning the overall distribution of those with denied, withdrawn or certified cases for both full and part time statuses. The tree map clearly shows that there are significantly more full-time positions available than part time.  However, despite this disparity, it appears that those seeking part-time jobs may be more likely to be successful in becoming certified.

Figure 3 is a very useful illustration of the relation between certified cases with Full-time or Part-time status and average prevailing wage.

![Wage~Case~FullTime](https://github.com/zjiwei/Tableau-Final-Project/blob/master/Wage~CaseStatus~FullTime.PNG)

**Figure 3. Case Status by Position Type**

### Using Metadata

Using Tableau’s metadata functionality, we were able to create a hierarchy of folders, changing data types and creating calculated fields. Our data can be saved and published while keeping its interactive features.

We were able to use Tableau to detect the presence of large outliers in the data. For the variable ‘Prevailing Wage’, using the Create Groups function, we found that a record had a value of almost 7 billion dollars. Many other applications had prevailing wage values in the hundreds of millions (see Figure 4 below). For our analysis, we wanted to exclude these records, since our goal is to help MSBA students understand the dynamics behind the visa process in the US, and that we probably won’t be applying to jobs making over a billion dollars per year after the program.

![Filter](https://github.com/zjiwei/Tableau-Final-Project/blob/master/Filter.png)

**Figure 4. Outliers using Metadata Functionality**

### Using Maps and Geographical Data in Tableau - Location of Jobs

While Tableau is extremely useful in many areas of data processing and data visualization, one area we found that Tableau was exceptionally powerful was in using geographical data. For example, there is information about worksites in our dataset, but each row contains both cities and states. Using Tableau, we can use custom split to divide them into cities and states which will play a key role in our further analysis. In Tableau, it is easy to change our data into types, including the extremely useful geographical, according to our needs.

We are able to take a textual field like “worksite” and modify it into both City and State Worksite fields. Using these new fields, we can start to learn about the geographical characteristics of applicants. Figure 5 shows the location of applicants, using the size of the bubble to signify the number of applicants in that location.

![Location~H1B](https://github.com/zjiwei/Tableau-Final-Project/blob/master/Location~H1B.PNG)

**Figure 5. Location of Applicants**

We identified the location as an important factor to investigate because job hunting in locations where H1B Visa applicants have had previous success could indicate an area where their skills are more in demand. Tableau provides visualization methods that are useful and extremely easy to implement. We can use symbol maps to show the information more directly. According to the graph above, we can know there a number of opportunities in the state of California, New York, and Texas. We hypothesize that this may be due to the fact that these locations have more jobs that are technology driven and are seeking out talent both foreign and domestic.


### Using Maps and Geographical Data in Tableau - Salary
In addition to where H1B applicants are most likely to get jobs, we would like to investigate the average wage of certified applicants in different states. Figure 6 below shows that there is little difference in wage in most states and the highest average wage is located in the state of New Mexico. 

![Location~H1B~Wage](https://github.com/zjiwei/Tableau-Final-Project/blob/master/Location~H1B~Wage.PNG)

**Figure 6. Prevailing Wage by State**

Our dataset also provides information about the types of jobs. This allows us to further analyze the types of jobs that are receiving the most applicants and may be the most competitive. Figure 7 below shows the number of applicants for each job type. Surprisingly, the jobs of most applicants are related to computer or software. This bodes well for our fellow MSBA colleagues as our skillsets may be transferable to many of these positions.

![H1B~Soc%20Name](https://github.com/zjiwei/Tableau-Final-Project/blob/master/H1B~Soc%20Name.PNG)

**Figure 7. Number of applicants by Job Title**

Focusing on the certified group and including the data of wage, we can know that there is a great difference in different types of jobs. Thanks to the interactive interface in Tableau, we are able to know details of each point. Figure 8 shows a screenshot of this useful, interactive feature.

![CWS](https://github.com/zjiwei/Tableau-Final-Project/blob/master/CWS.PNG)

**Figure 8. Certified Candidates Wage and Job Types**

### Challenges
We faced a few challenges when analyzing this dataset. One roadblock faced when starting was identifying major outliers in the dataset. When doing preliminary analysis, we got what seemed at first to be strange results. Figure 9 below shows one example of a curious and unusual result we found.

![Wages%20of%20applicants](https://github.com/zjiwei/Tableau-Final-Project/blob/master/Wages%20of%20applicants.png)

**Figure 9. Wages of applicants.**

The histogram above for the prevailing wage variable in our dataset does not make any sense. It seems to say that there are about 3 million jobs that pay $0 million, and none that pay more, but the axes are not appropriate. After trying to adjust axes for a while, we realized that the problem arose from outliers in the data. There are jobs that post prevailing wages of over a billion dollars, but there are so few of them that they are invisible in the above histogram (count of 1 or 2 versus 3 million for the first bin). Therefore, we had to exclude, as mentioned above, the applications with the highest prevailing wage. After doing so, we got better results and were able to proceed with the rest of our analyses. Below is a more appropriate histogram, set to exclude prevailing wages above $500,000. Figure 10 shows this result.

![wages%20less%20than%20500k](https://github.com/zjiwei/Tableau-Final-Project/blob/master/wages%20less%20than%20500k.png)

**Figure 10. Wages <500k**

### Conclusion

As soon to be MSBA graduates who will be seeking full-time employment and (many of us) in need of work visas, our group had a personal and vested interest in what the data had to say. We were interested in questions involving whether or not full-time or part-time jobs were more common, what salaries we could expect for a given job type, what job titles are most common for visa applicants, and where those jobs occurred.

Additionally, our group was interested in learning how to use the Tableau software and the ways in which this program could be used in our future jobs to create clean and powerful visualizations for our clients and organizations. Using Tableau, we were able to create mapping visuals with just a few clicks of a button where performing the same task in R or Python would require multiple lines of code to be written. The flexibility and intuitiveness of Tableau was surprising to each member of our team.

Lastly, what does this mean for our fellow MSBA colleagues? Overall, we found the data to provide a mixture of good and bad news. While it was encouraging to see tens of thousands of applicants be accepted, there were also a large number of denied applications. Without more information regarding why these applications were denied, it’s tough to say how best to improve an applicant’s chances of being accepted.

However, there was also good news in the data set. We found that many of the top jobs center around skills that the Business Analytics program will provide us with. We learned about where you are most likely to become certified (New York, California, and Texas) and where you are most likely to receive a high salary (New Mexico). This information will become useful when applying to jobs.

We believe this project provided valuable skills as well as a better understanding of the US Visa landscape. Both points will be valuable to us moving forward in the program and as we begin our professional careers.
