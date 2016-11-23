# CrowdStory

Milestone 1 | Special Topics In CS - Crowdsourcing | KAIST | 2016

## Team Information
Goh Wei Xiang, Liu Ching, Miroslav Masat, Oscar Johanson

## What is the problem your team is trying to solve? (one sentence)

The problem we are trying to solve is a collaborative content creation using the crowd.

## Why is this problem important?

People may want to create some stories. A bloger need story to attract reader,a  compony can use stories to express their culture or history to public, a movie director may want to gain a cool script which is close to people’s life. However, making a story is a hard work for now, relying on experts, usually work alone and take a long time. Every crowd have their own experience that can contribute to a story, or there might be talented crowd who are talented story tellers but it is hard for them to write a long story by themself. SCHEHERAZADE is a crowdsourcing platform that reach to crowd to create a sotry graph plots. However, they tend to automatically generate the story by using the rough graph plots, which can limit the story structure and also lose the beauty of literature. So our idea is to provide a system that can both asist the crowd to create a structured story and also the final story written in their own language. 

* [Story Generation with Crowdsourced Ploted Graphs](www.cc.gatech.edu/~riedl/pubs/aaai13.pdf)

* [Crowd Control: our crowdsourced science fiction novel, starts here](https://www.cnet.com/news/crowd-control-our-crowdsourced-science-fiction-novel-starts-here/)

  ​

## Why use crowdsourcing for the problem? Why not use machines or a small group of experts?

* Generation of story content is both slow and expensive. If we can lower the price and speed up the process, we might reinvent this field. Writting a story is a knowledge-intensive process and offering a diversity of ideas can really help to bring a good story. Crowdsourcing can definitely help to decompose the story and enrich it, piece by piece, with no bias or predefined writting style. As opposed to experts, that can be of limited availibility and given singularity, we offer much more flexible and available workforce with diverse opinions. All this can be offered for a fraction of cost of the work of experts.

## For the identified problem, discuss with your teammates what specific challenges exist. State these challenges as "How might we..." questions. For example, for [the ESP game](http://dl.acm.org/citation.cfm?id=985733), questions might include *"How might we make the game fun so that people play multiple sessions?"*, *"How might we ensure that there is always a partner for any player at any given time?"*, and *"How might we encourage players to type in accurate labels?"*. List at least 10 "How might we..." questions for your problem based on the team brainstorming. 


* How might we motivate crowd to deliver the best job?
* How might we recruit workers?
* How might we decompose the story into small enough but meaningful chunks?
* How might we prevent one of the worker to dominate the whole story?
* How might we control the flow of the story in parallel way?
* How might we engage the requester to evaluate a story
* How might we attract the crowd to keep writing and generating good stories without spamming? 


## In your team, discuss how you might address these questions with crowdsourcing. Then pick the three most promising solutions overall. These solutions need to be rough and diverse at this point. For each idea, answer the following:

### What is the one-sentence summary of the idea?

On demand crowdsourcing generate story book.

### Describe a scenario from the requester's point of view. Think how an imaginary requester might use the system. How do they create a task? How do they review results and successfully end the task? 

1. Requester decides to obtain a creative story by minimizing the cost using our system.
2. Requester comes to the website and specifies the theme, characters, length and optionally even main storyline.
3. Requester can oversee the whole process as the new pieces of story are being generated and also give some reputation to best workers, allowing them to contribute more.
4. Requester can at any time stop the task, if he feels that the objective was fullfilled. After closing editing of the story, the final version is released and authors of resulting paragraphs are also listed.

### Describe a scenario from the worker's point of view. Think how an imaginary crowd worker might use the system. How do they come into the system? What is the task experience like? What motivates them to keep contributing? 

1. Workers will register to the platform and optionally can express their interest to be notified by the types of stories they could be interested in contributing.
2. After picking an interesting story assignment, the worker can suggest a paragraph or revise already existing one.
3. Worker can then also evaluate contributions of other workers and help to shape the story with their own experiences can creativity.
4. Workers are kept motivated by seeing their paragraphs being upvoted and by requestor appretiation via awarding reputation.
5. Motivation come when no one can guess what is the ending and worker want his/her creativity may become people’s favourite.

## Analyze the idea using the seven dimensions above. Make sure your team's three ideas have clear differences in some dimensions.

### Motivation - why would a crowd worker do this?

* For those who are interesting in writing but can not fulfill a conprehensive story by their own, they can cooperate with each other and contribute to a good story. 

* Crowd who contribute to the final story can gain good reputation and they can see their name on the author list.

### Aggregation - how are results from multiple workers combined?

* Multiple instances of one paragraphs are allowed, while the voting system can help to determine which instance will stay.

### Crowd pool - you are required to use a VOLUNTARY OR INTRINSICALLY MOTIVATED CROWD, but please be more specific.

* Crowd pool consists of writers that want to get a practice and free exposure of their writtings. 
* They can also gain inspiration from fellow writters and hence, enhance their skill using our platform.
* Point system is implemented in our system to motivate our workers.
* Each worker is given a same amount of starting point and they can made their own decision with the points.
* Worker can earn extra point by being active in our platform.

### Quality control - how to ensure valid results?

* Multiple mechanisms will be employed. Reputation system and extent to which selected workers will be able to contribute are the main ones. There will be limited oprion of deleting the content as instances of paragraphs can outperform each other but never be removed forever.

### Human skill - what kind of human skill is required to complete a task?

* No special skill is needed except the ability to write gramatically correctly. Willingless to iterate and optionally get rejected is appreciated.

### Process order - in what order is the work processed between computer, worker, and requester?

* The process starts with a requester that submits an assigment for workers to work on. After being accepted by administrator, the task will be available for workers to review and join. After joining, the workers can suggest new paragraphs or iteratively enhance. 

### Goal visibility - how much of the overall goal of the system is visible to an individual crowd worker?

* We give whole visibility to crowd, from the goal, working process. And becuase workers sure a synchronous writing workspace so the result is updated in real-time to all the crowd.

