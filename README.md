# attrition_analysis1

EMPLOYEE ATTRITION 

Dataset Analysis 

OBJECTIVE 
This report presents a comprehensive analysis of data sourced 
of Employee attrition. The primary objective of this analysis 
is to uncover key insights, trends, and patterns within the 
dataset, providing valuable information of employees leaving 
the company

Findings:
- Total number of attrition: 
select attrition,count(*) from employee_attirtion_new 
group by attrition; 
Attrition NO: 1477 
Attrition YES: 199

 - Attrition count according to gender: 
select gender,count(*) from employee_attirtion_new 
where attrition ='yes' group by gender; 
Female - 592 
Male – 885

- Attrition yes count according to Marital status: 
select maritalstatus,count(attrition) from 
employee_attirtion_new where attrition='yes' group by 
maritalstatus,attrition; 
Single - 114 
Married - 61 
Divorced - 24

- Attrition yes count according to job satisfaction 
level: 
select JobSatisfaction,count(attrition) from 
employee_attirtion_new where attrition='yes' group by 
JobSatisfaction,attrition order by JobSatisfaction; 
JobSatisfaction, count(attrition) 
1 - 52 
2 - 42 
3 - 60 
4 – 45

 - Attrition yes count according to income 
catogery: 
select income_cat,count(attrition) from 
employee_attirtion_new where attrition ='yes' group by 
income_cat; 

- Attrition yes count according to different 
educationfield: 
select educationfield,count(attrition) from 
employee_attirtion_new where attrition='yes' group by 
educationfield order by count(attrition);

- Attrition yes count according to different 
department: 
select department,count(attrition) from 
employee_attrition_new where attrition='yes' group by 
department order by count(attrition);

- Attrition yes accord jobinvolvement rate: 
select jobinvolvement,count(attrition) from 
employee_attirtion_new where attrition='Yes' group by 
jobinvolvement order by jobinvolvement
