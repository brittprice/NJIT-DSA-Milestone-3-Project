# NJIT-DSA-Milestone-3-Project
This is the README file for my Milestone Project 3 (final project) for the NJIT Data Science and Analytics Certificate Program.

I am someone who is changing careers in my 30s. I chose the path of using a bootcamp program in order to obtain the knowledge needed to change careers as going back to school full time and getting another undergraduate degree wouldn’t allow me to continue to maintain a work-life balance, pay for said program, and keep up with rent and bills. I have done all the right things—gotten an internship, done well in classes, worked with my career coach, updated my resume, gotten some actual real-world experience under my belt and even done a few paid short-term projects for various companies, however, when it’s come to finding a full-time job in data science I have been hitting roadblocks left and right. 

-	Is it because I didn’t get my undergraduate degree in data science, 
economics, statistics, or finance?
-	Is it because I don’t have a master’s degree? 
-	Is it because I'm a female? 
-	Is it because I don't have prior work experience?

Since we were free to choose a dataset on any topic (as long as the set was longer than 100 entries and included over 4 features) I decided to do an analysis of a job placement dataset to find out what variables are most likely to impact job placement.

I feel like this will be helpful knowledge for other people on the job hunt.

This is the dataset from Kaggle that I chose:

https://www.kaggle.com/datasets/ahsan81/job-placement-dataset?resource=download

About this file

This file contains different attributes of the candidates educational history and work experience. The detailed data dictionary is given below:

Data Dictionary

gender : Gender of the candidate

ssc_percentage : Senior secondary exams percentage (10th Grade)

ssc_board : Board of education for ssc exams

hsc_percentage : Higher secondary exams percentage (12th Grade)

hsc_borad : Board of education for hsc exams

hsc_subject : Subject of study for hsc

degree_percentage : Percentage of marks in undergrad degree

undergrad_degree : Undergrad degree majors

work_experience : Past work experience

emp_test_percentage : Aptitude test percentage

specialization : Postgrad degree majors - (MBA specialization)

mba_percent : Percentage of marks in MBA degree

status (TARGET) : Status of placement. Placed / Not Placed



After reviewing the dataset I found that all candidates had a graduate degree, so instead, I proposed the question of “is work experience an accurate predictor of job placement?”

Features to choose to predict a job placement:
gender, work_experience, mba_percent, emp_test_percentage, undergrad_degree, specialisation

Target variable:
Status “Placed”

I ran a few models (A K-Nearest Neighbors, Gradient Boost classifier and a Random Forest model) and chose a Gradient Boost classifier as my model because it wasn’t over or underfitting. The model was stable with a  training score of 0.994 and a testing score of 0.852.
I also checked for feature importance and found that:
1. Undergrad grades seem to have the highest impact on job placement
2. Followed by grades during their graduate courses
3. Work experience didn’t have as much of an impact as expected, although it was still statistically significant
4. People who went into Marketing & Finance had better job placement than people who went into Marketing & HR

In conclusion, a lot of factors affect job placement. Work experience doesn't have as much as an impact as I originally thought. Going into finance seems to be a good path right now for those that aren't sure what they want to do with their careers (undeclared undergrads, I'm looking at you). I'm happy to see that the evidence in this dataset is showing me that gender isn't impacting job placement (yay, progress!). In short, do well in school. Take it seriously. Doing well in school seems to have the biggest impact on landing a job!
