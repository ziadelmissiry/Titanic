# Introduction 
The Titanic is one of the most iconic disasters in history and its story captivates audiences to this day. With advances in data analysis, it is now possible to analyze data from this tragedy to gain valuable insights with the help of Python. This essay will analyze the Titanic dataset with Python to provide a better understanding of the voyage and the lives lost. Through these data analysis techniques and Python, we can gain a deeper understanding of the circumstances behind the tragedy and the people involved.

Data analysis is the process of analyzing data to extract useful information and insights, and Python offers a range of solutions for this task. Python provides libraries, such as NumPy, pandas, and scikit-learn, that contain various functions for handling and analyzing data. Furthermore, it is easy to use the powerful plotting libraries, such as Matplotlib and Seaborn, to generate visualizations to better understand the data. In addition, powerful Machine Learning algorithms, such as support vector machines, random forests, and unsupervised learning algorithms, can be used to gain insights from structured data. By combining all of these capabilities, Python is a powerful tool for data analysis (Henderson et al.). 

# General Data
 Using pandas in python will allow for greater accuracy when predicting an outcome. The library pandas offers multiple model tools including appropriate frameworks for creating models based on large data sets such as those from the Titanic. Whenever I'm introduced with a dataset I like to understand the dataset and have a little bit of background knowledge on it. This dataset has a count of 891 meaning that there are 891 objects in the list and there are 177 nulls in age and 687 in Cabins and 2 in embarked as seen in figure 1, later on we will be removing the nulls to conduct more tests on the data.  Figure 2 in the appendix shows further background knowledge on the data we are examining such as max minimum and the count of passengers embarking from certain areas. 

# General Data: How to break it down
	 Examining records from Titanic’s voyage may be a helpful first step; preparing these records can include looking at each individual passenger’s age, sex, class ticket type etc. When examining these categories in order to better understand how they may have played a role in determining survivor status on board, it is evident that certain features such as ‘Age’ and ‘Class’ Ticket Type' had more influence than others like ‘PassengerId', 'Ticket' and 'Name'.

# Male VS Female 
	One notable pattern that quickly becomes evident through a descriptive analysis of titanic passenger data is that more women survived than men during this debacle; 81 out of 891 female passengers survived compared to 109 out of 577 male passengers. Although these figures seem straightforward at first glance, further investigation reveals that there was a nuanced element at play here as well. Figure 3 shows two histograms depicting age distribution for both female and male survivors wherein it can be seen that although women had better chance of surviving when they were between 14 and 40 years old, men had better likelihoods for survival when they were between 18-30 years old. This suggests that other factors besides gender likely played some role in determining who was able to successfully evacuate off board before tragedy struck. In order to gain deeper insight into all these various facets associated with Titanic's fateful journey an evaluation across categories such as passenger class, port origin/destination etc must also take place. 

Passenger Class
We begin by examining simple statistics like mean number of survivors versus non-survivors in each class as well as other factors such as gender or age group: for instance Here we see clearly that the passenger class contributes greatly towards a person's chance of survival through having significantly higher numbers in 1st Class compared with lower classes; among 1st Class passengers alone there were 136 out of 216 total survivors- significantly more than both 2nd (87) and 3rd Class (119) as seen in figure 4. This establishes a strong correlation between one's chances of surviving and one's assigned seating group within the boat's compartmentalization design. Moreover, it may also indicate that many 3rd member cabin passengers may have had less access to lifeboats than their richer counterparts because some boats could only hold a limited number of people at once.

Port / boarded

According to an analysis made based on figure 5  on the available data, women had a higher chance of survival depending on which port they boarded from: Queenstown or Southampton had much greater rates than Cherbourg; however, men onboarding from Cherbourg had better chances than those who departed from either Queenstown or Southampton. This is likely due to discrepancies in the way first-class passengers were taken care of versus lower classes—it was already known that more women made it out alive largely because they were prioritized over men when it came time for evacuation—but how these ports are connected remained unknown until now. 


Relatives 
This analysis of the Titanic dataset provides an insight into how relationships between individuals, especially family members, can influence the chances of survival during a disaster. Figure 6 demonstrates that passengers with less than 1 or more than 3 relatives on board had lower levels of survival rate compared to those with 1 to 3 relatives. This suggests that having a handful of close friends or family members around during such difficult times may improve one's odds of success and thus should be considered when preparing for similar types of scenarios in the future. In fact, 76% did not bring any parents or children and 68% did not bring any siblings on board as reported by this data set. One could speculate that those who did bring relatives had assistance obtaining necessary resources during the evacuation procedure which could account for increased survivability; however, further research would need to be completed in order to sufficiently explore this concept.

Decision tree
Using the data visualized in Figure 7, a comprehensive analysis of the Titanic dataset can be made with Python. Each box represents impurities in the data using the Gini index. It is clear from this decision tree that by far, passengers who traveled first class had a much higher chance of surviving than those traveling second or third class. Furthermore, based on the data presented, one can conclude that female passengers have a notably higher survival rate than male passengers regardless of their ticket price. This insight has been re-emphasised multiple times over many years following this disaster; however it is interesting to see how true it still holds when examined with such clarity by way of analytic tools such as Python and its associated analytical libraries (in this case sklearn's DecisionTreeClassifier). With regard to ticket prices overall, it appears that directly correlated with expected social hierarchies, passengers who paid lower fares were at significantly more risk irrespective of gender or class designation when compared to those traveling with more expensive tickets.

K-Means Cluster 
To further explore the data I employed unsupervised learning algorithms - specifically k-means clustering - to find patterns and correlations between passenger characteristics such as fare price, age, and survival rate. Utilizing the elbow method, I found that four clusters accurately represented my data set (Figure 8). I then took these results further by plotting them against each other while visualizing any correlation they may have had with one another – namely, the relationship between age and survival or fare price and survival rate (Figures 8). The resulting graphs showed a distinct grouping based on the passenger's age group or purchase price group. Clearly there were established trends within how certain factors affected survivors during the sinking of the titanic; however more research would be needed to understand their causation. As such further explorations using unsupervised learning techniques could explore these tendencies much more thoroughly. Nevertheless this initial analysis gives us strong preliminary evidence that supports our hypothesis that age group and fare prices significantly impacted passengers’ chances at surviving during this disaster.

Conclusion 
In conclusion, the data analysis performed on the Titanic dataset using Python demonstrates that certain features - namely age, class, fare, and sex  had more influence than others like PassengerId, Ticket, and Name. Women had a better chance of survival when they were between 14 to 40 years old whereas men had higher likelihoods for survival when they fell within the 18-30 years age bracket. Additionally, another key factor determining passenger chances of survival was their class: passengers in first-class generally survived at much higher rates compared with other classes since their needs were catered for differently. Lastly, there is also evidence which suggests that depending on which port the passengers boarded from (Queenstown or Southampton versus Cherbourg), this too influences whether or not the passenger will survive; Female passengers placed onboard from Queenstown and Southampton tended to have lower survival rates than those who embarked from Cherbourg while males show contrary results with better chances of surviving as long as they embarked at Cherbourg versus either Queenstown or Southampton. Thus, these findings suggest that certain factors play a crucial role in influencing a person's chances of survival onboard the Titanic and ultimately paint an impartial picture depicting how devastating this tragedy was for all involved.
























Appendix 

Figure 1


                  Total              %
Cabin          687             77.1
Age            177               19.9
Embarked     2                  0.2
PassengerId  0                  0.0
Survived         0                  0.0

(Donges, 2018)

Figure 2


There are 177 nulls in Age and 687 in Cabins
PassengerId    891
Survived       891
Pclass         891
Name           891
Sex            891
Age            714
SibSp          891
Parch          891
Ticket         891
Fare           891
Cabin          204
Embarked       889
dtype: int64
****************************************************************************************************
Death count = 549
1st class = 216
2ed class = 184
3ed class = 491
Southampton = 644
Cherbourg = 168
Queenstown = 77
Parch Max = 6
Parch Min = 0
parch = 0 = 76.0942760942761%
parch = 1 = 13.243546576879911%
parch = 2 = 8.978675645342312%
parch = 3 = 0.5611672278338945%
parch = 4 = 0.44893378226711567%
parch = 5 = 0.5611672278338945%
males count = 577
female count = 314 
Min Age = 0.42
Max Age= 80.0
passenger under 18: 139
passenger over 18: 575
Figure 3
