# Employee Attrition

# Introduction

## Research Paper on Employee Attrition

I recently went through an research paper on [employee attrition](http://kth.diva-portal.org/smash/get/diva2:1461317/FULLTEXT01.pdf). Here are few highlights I could capture. 

### Few keypoints

- **Employee satisfaction is inversely related to Attrition.**


- **Effect of Attrition on a company.**
    - Negative effect on producticity.
    - Knowledge loss, gone with the employee.
    - Increase in workload for remaining employees.
    - Negative impact on companies morale.
    - More expense on process for hiring and training new employess.
    

- **Why employess leave job(internal reasons)?**
    - Disatisfaction
    - No-commitment to the company


- **Factors affecting satisfaction(internal).**
    - Connectedness to others 
    - Feeling of belonging somewhere.
    - Feeling of support from organization.
    - Resonable workload.
    
    
- **Using ML in HRM (Human Resource Management).**
    - Small data, and sometimes not even recorded.
    - Decision made by HR have heavy consequences.
    - Measuring performace is hard, depends on teamwork. And individual performance is difficult to extract from teams performance.
    - Hiring/Firing is not only based on tangible reasons but also on psychological relations between employees.
    - ML algorithms can be biased and can not take into account of everything about future employees for instance race can cause bias. *Author also gives example of Amazon removing gender column to remove biases.*
        

**ML Model Interpreteability**

Local: Relation between prediction and small subsets of data.

Global: Relation between prediction and large segment of data. 

Global helps to understand how the model works as a whole. Local can be more descriptive of how model is performing.

As far as the ML alorigthms, author has used SVM, Logistic Regression and Random forest and did comparision between them. 

(*Again these all info's are something I took as a note from the research paper I mentioned above and not my work.*)
   
## About Data

The data is publicly available in kaggle @ https://www.kaggle.com/colearninglounge/employee-attrition.


## Few EdA's on the project.

### Correlation Between Features

![img](https://github.com/nibukdk/employee-attrition/blob/master/Imgs/Correlation%20Heatmap.png)

Lets see as expected job level has postive and higher correlation with other features like years expeirence, monthly income and the department people are working on. 

Looks like relationship with current manager gives a good boost on your chances for your current role and you continue on having your job. 

### Distribution Plot

Histogram plots to check if some properites are sure fire way to distinguish attrition, but lets first drop this employee count column it has only one value.


![img](https://github.com/nibukdk/employee-attrition/blob/master/Imgs/Distribution%20Plot.png)

Unfortunately, it seems the values are quite mixed to be sure. But if we look closely, attrition(value "Yes") are higher for employess with lesser monthly income, less total_working_years. And if we check age column either younger employees who are just starting thier career or older employees at retiring age are more likely to leave company than the middle aged ones. 

Interestingly if u check that num_of_companies worked, chances of leaving or staying are same as the number of companies increases.


### Qualification, Experice and Salary

![img](https://github.com/nibukdk/employee-attrition/blob/master/Imgs/Employee_Qualifications_n_Salary.png)

Salary does increase with qualifications. But college graduates seems to have more salary with less experience in comparision to those bachelor's degree. 


### Satisfaction LVL vs Attrition




Attrition = Yes |  Attirion = No
:-------------------------:|:-------------------------:
![img](https://github.com/nibukdk/employee-attrition/blob/master/Imgs/Satisfaction_Lvls_n_Attrition_Yes.png) | ![img](https://github.com/nibukdk/employee-attrition/blob/master/Imgs/Satisfaction_Lvls_n_Attrition_No.png)




