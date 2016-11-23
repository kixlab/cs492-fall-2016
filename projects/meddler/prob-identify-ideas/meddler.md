
CS492 Crowdsourcing - Final Project: **Milestone 1** (2016-10-05)

- 20165192 Sunggeun Ahn (topmaze@kaist.ac.kr)
- 20165161 Young-Min Baek (ymbaek@se.kaist.ac.kr)
- 20163703 Sungjae Hong (yain@kaist.ac.kr)


----------



Problem Identification and Ideas
=======================

## A. Problem Identification

### PROBLEM STATEMENT

#### What is the problem our team is trying to solve?

- **Problem**: Unfair and ineffective environment for learning and education
- **Goal**: Fair opportunity of effective education using crowdsourcing

![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475761390341/2016-10-06-images---cs492-new/01.png)

　

#### How do we know this problem exists?

+ Unfair opportunity and environment can lead to the difference in the level of education.
+ Purchasing learning materials and registering courses have costs. 
+ Existing learning materials are tedious for continuing study.
 - Fixed question (problem) pools of usual textbooks, workbooks, online-learning services have limitations in diversity and creativity.


![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475761402282/2016-10-06-images---cs492-new/02.png)

+ According to the survey of *Statistical Office of Korea* 
 - Private education costs increase as household income increases.
 - Regional differences cause differntials of private education costs.

![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475761410979/2016-10-06-images---cs492-new/03.png)

![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475761418096/2016-10-06-images---cs492-new/04.png)

(통계청 보도자료(A Report of National Statistical Office), "2015년 초·중·고 사교육비조사 결과(Private Education Costs of Korean Elementary, Middle, and High School Students in 2015),” 2016)


+ Based on our personal experience,
 - *"When I was a tutor for children, I could observe that there are a lot of difficulties for **underperivileged students to study equally** with other students."* (Sunggeun Ahn, 2008)
 - *"There are many people who want to learn new things at a later age than others. For example, my parents want to study Chinese or English, or some elderly people can start learning programming. However, if they **missed the right time to get the education**, the way to study has a high entrance level (or barrier)."* (Sungjae, Young-Min)

　

### CROWDSOURCED APPROACH

#### Why do we use crowdsourcing for the problem?

![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475761433629/2016-10-06-images---cs492-new/05.png)

### CHALLENGES

#### Challenges of a crowdsourced learning system

1. *[Motivation]* How might we motivate voluntary learners to study something using our platform?
2. *[Motivation]* How might we make people (workers or requesters) write test questions (i.e., problems) voluntarily?
3. *[Quality control]* How might we guarantee the quality of test questions which were made by voluntary workers?
4. *[Diffilculty control]* How might we identify and provide a proper level of problems for each learner?
5. *[Pool generation]* How might we effectively recruit people who want to study at first?
6. *[Quality control]* How might we handle (filter out) wrong information?
 - Wrong problems made by workers
 - Spam problems/answers/messages by advertisers or saboteurs
7. *[Environment/Interface]* How might we guarantee "Quality Learning Service" for requesters and workers?
 - Ease to use: How might we make our interface intuitive and simple?
 - Mobility: How might we build our platform that can be accessed and used anywhere?
 - Fun/Enjoyment: How might we give pleasure to learners without any obstacle?
 - Sustainability: How might not we make our service boring? How might we effectively maintain already existing users?
8. *[Aggregation]* How might we utilize the aggregated learning data for the better learning for next time (or next cycle)?
9. *[Copyright]* How might we deal with copyright issues of the user-provided learning materials (i.e., problems, questions, and solutions)?
 - If a problem provider makes a test question using existing textbooks
10. *[Responsiveness]* How might we control the response time?
 - What is an appropriate interval for pushing messages with problems?
 - When do we have to aggregate submitted data (questions and answers) from users?

　




## B. Ideas & Solutions

### IDEA 1: *CROWDSOURCED EXAM EVALUATION*


#### Summary of the idea

+ ***To estimate the levels of difficulty of exam, request evaluation to learner crowd***

![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475761442353/2016-10-06-images---cs492-new/06.png)

#### A scenario from the requester's point of view

- Requesters join with basic informations
	- What's your Job?
		- teacher, part-time private tutor, workbook maker
	- Why you need problem evaluation? (Enable multiple choice)
		- to set exam questions, to delvelop good learning materials
	- Who's the target student? (Enable multiple choice)
		- middle school, high school
	- What's the target subject? (Enable multiple choice)
		- English, math, science, etc.
- Request process
	- Take **a problem image** with their smartphone camera
		- The image only include one problem 
	- Upload a image
	- Insert problem information
		- is it objective problem?
			- currently, we may support objective problem only. 
		- number of answer
		- number of correct answer
		- self estimation of level of difficulty (1-5 likert scale)   
	- Set a correct answer
	- Select target student 
	- Select subject category
	- Set a deadline
- Get results of a single request
	- Worker's information
		- distribution of age, job, academic abillity   
	- Statistical results: mean, median, standard deviation 
		- **quantitative factors**: error rate, completion time
		-  **qualitative factors**: subjective difficulty, subjective annoyingness
	- A requester can see filtered result
		- ex: resutls of 'job: middle school student' 'academic ability: level 3'
	- Distribution of answers (ex: no.1 - 30%, no.2 - 20%, no.3 - 50%)
	- Check workers comment
		- if there are good comment, a requester can give a point to worker  
- Combine the results of problem set
	- Select a set of evaluated problems
	- Set a academic level of requesters students
		- ex: level 1 - 30%, level 2 - 60%, level 3 - 10%) 
	- Get a estimated results of exam
		- Mean, median, standard deviation

#### A scenario from the worker's point of view

- How do workers come into our platform?
	- Keywords for accessing our platform 
		- Mobile study application
		- Free problems for study
	- Workers join with basic informations
		- What's your Job?
			- elementary/middle/high school student, etc. 
		- How old are you?
	- Workers should select the target subject
		- to select the target subject, workers must take a simple test for estimating acamemic ability 
		- also, a worker can receive requests only about the selected subjects. 
- Receiving a request
	- Passive receiving
		- If a worker set enable to get a push alarm, he/she can get push alarm for evaluation request
		- A worker can access a problem by clicking recieved push alarm.
		- Also, a worker can set a recieving period and time
	- Active receiving
		- A worker can access a request by clicking "receive button" on the list of target subject
- Evaluating a problem
	- Solve a problem
	- Evaluate a level of 
		- Difficulty, Annoyingness, Quality
	- Comment to requester (if a worker want)
- Checking current status
	- Solving history
		- answered problems, number of solving, error rate 
	- Current level of academic ability
		- level of academic ability is refleshed when a worker solve a problem
		- academic ability is evaluated on each subjects
	- Point
		- point is achieved for every work
		- Also a worker can recieve point from his/her comment
- Reward
	- A set of high quality problems
		- a worker can use point for getting a set of high quality problems in document format
	  	- Level of quality is evaluated from other workers evaluation 

#### 7-Dimension Analysis

![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475762009073/2016-10-06-images---cs492-new/21.png)

　

-----

### IDEA 2: *FORUM-LIKE CYBER PLATFORM*

#### Summary of the idea

+ ***Providing forum-like cyber platform to help translation of an English sentence***

![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475761457612/2016-10-06-images---cs492-new/08.png)

#### A scenario from the requester's point of view

##### A. Creat a task

+ A requester uses a smart device to login to the platform.
+ When a requester logs-in, he or she needs to choose the best translation from the given translations of a certain English sentence, which is one of other requests in the platform.
 - Choice of the sentence is based on the number of evaluations; if the request on the sentence was given a long time ago and small amount of evaluations are done, the sentence is more likely to be shown.
 - In the validation phase, a requester can ‘Report’ translation for malign action and duplication. If the number of reports come to the certain translation, it will be deleted.
+ After log-in, a requester can push ‘Create’ button to submit a new sentence to be translated. He or she can choose a duration of the request, maximum to 2~3 days.

##### B. Review results

+ A requester can see a bulletin board-style structure after submitting a request.
+ Each post shows translations of a requested sentence, sorted with the number of recommendations for each translation with the status of a translator, which shows how this translator (worker) translates well.

##### C. End the task

+ A requester can choose one (or more) translation, then translators will get some points.
+ A requester can give a rating to the chosen translation (or a total service)


#### A scenario from the worker's point of view

##### A. Come into the system

+ A user of the platform can be both a requester and a worker. Thus, the way to start the system is same as that of a requester.

##### B. Task experience

+ Click ‘Translate’ button after the log-on. Then a sentence will be given for the translation.
+ If a worker wants to translate, click ‘That’s my work’ and suggest a translation. Otherwise, click ‘Pass’ button to find other sentences.


##### C. Motivation 

+ Any kinds of rewards: reputation system, badges, titles, etc.
+ Workers also can improve English skills by doing other ones’ translation.


#### 7-Dimension Analysis

![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475761593117/2016-10-06-images---cs492-new/19.png)

　

-------

### IDEA 3: *1 DAY 10 QUESTIONS*

#### Summary of the idea

+ ***“My curiosity can be a new study material (problem) for others.”***
 - Sharing and collaborating the learning experience & progress with other learners who have the same educational interest.


![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475761464943/2016-10-06-images---cs492-new/09.png)

#### A scenario from the requester's point of view


##### A. Join our platform and select a study topic of interest

+ Every learner can freely sign up for a membership of the platform.
+ Before getting started, a user has to select some of his or her study topic (e.g., English, Chinese, programming) to easily find people with same interests.


##### B. Write a simple test question

+ A requester who wants to share a problem that will help others can upload a new test question to our platform.
+ The interface allows a simple and basic form to make a test question to make problems solvable within a short time.

##### C. Mark submitted answer

+ After the time period is up, a requester can receive the aggregated answers written by other people who had got the requester’s problem.
+ As a requester knows the correct answer (solution), the submitted answers can be marked.


##### D. Manage own reputation

+ A requester can be an online teacher if his or her questions get good quality ratings on average. It can be used as a reputation.
+ A requester can be added to other learners’ Favorites list.

![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475761515699/2016-10-06-images---cs492-new/14.png)


#### A scenario from the worker's point of view

##### A. Join our platform and select a study topic of interest

+ Same as requesters

##### B. Receive arbitrary questions from other people 

+ A worker receives 3~10 push messages with simple test questions of registered interest.


##### C. Check the test question and solve it

+ A worker has to solve the given problem within the time allowed.
+ A worker can fill in the blanks with an answer and submit it.

##### D. Rate stars for the question (optional)

+ A worker can rate stars for the given question, and it will be reflected on the question provider’s reputation

##### E. Check my past history

+ Every learner has his or her own study history to look up.
+ Learners can do a review good problems which were added to <remember> list.

![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475761522923/2016-10-06-images---cs492-new/16.png)

　



#### 7-Dimension Analysis

![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475762804613/2016-10-06-images---cs492-new/22.png)　

(If the image is broken, use the hyperlink below)

[https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475762804613/2016-10-06-images---cs492-new/22.png](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475762804613/2016-10-06-images---cs492-new/22.png)

------

## C. Summary 

![](https://sites.google.com/a/se.kaist.ac.kr/online-image-storage-ymbaek/_/rsrc/1475761533465/2016-10-06-images---cs492-new/17.png)

