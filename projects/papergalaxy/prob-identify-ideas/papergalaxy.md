## Team 김조선
### 1. What is the problem your team is trying to solve?

We want to ease the reading experience of academic papers, so that the readers don’t have to go through same trial and error or difficulty someone else already went through.

### 2. How do we know this problem exists? Why is this problem important?

http://www.dailymail.co.uk/news/article-3223513/Is-science-hard-scientists-Experts-worry-academic-papers-unintelligible-NO-ONE-read-them.html#comments

According to the paper above, experts worry academic papers are now so difficult that even those who specialize them finds it hard to understand them. Richard Dawkins suggested that some papers can only be understood by ‘specialists in their respective fields. Furthermore, many students that we interview replied that, when they read something that requires lots of comprehension such as academic paper, it always helps them to ask someone who already read the paper. To be more specific, some interviewees replied that when they try to follow a math proof or reproduce the result of a certain experiment, sometimes the author leaves out  important assumption or some steps that make it very hard to follow. They could save a lot of time when they asked someone who has already gone through the similar trouble. 

### 3. Why use crowdsourcing for the problem? Why not use machines or a small group of experts?

Reading the academic paper and making meaningful annotations requires a very high-level understanding of the subject and the paper itself. Such tasks cannot be done by machines. Furthermore, there are millions of academic papers in many very different fields, which makes it impossible for a small group of experts to make annotations for every paper. Only the crowd (in this case crowd of experts I guess), can solve this problem.

### 4. “How might we …” Questions

How might we ensure that the annotation can be trusted?
How might we motivate people to actually make annotations or answer the question?
How might we show the annotations that were aggregated, so that readers can read it easily?
How might we bootstrap the system in the beginning so that people come to use our service?
How might we engage/satisfy people who prefer reading papers in hard copy?
How might we design the reading window to provide better reading environment?
How might we teach first-time users how to use the platform without distracting them from reading?
How might we ensure that the annotators/commenters are well-informed/experienced with the paper?
How might we maintain consistency excluding duplicate questions?
How might we implement a synchronous system that reduces the response time?
How might we assess the improvement that the system actually helps readers not to go through trials and errors?

### 5. In your team, discuss how you might address these questions with crowdsourcing. Then pick the three most promising solutions overall.

>### On Text Annotation

#### Summary
The idea is to show annotations and questions right on the text itself, so the readers can see annotations as they read the paper. 

#### Scenario (organic workflow):
*Requester’s Perspective: *
Mark is a graduate student in bioengineering department of KAIST. He is trying to reproduce the result of an experiment in a paper that was recently published on the NATURE journal. However, he soon realized that the descriptions in the paper was very rough and missing out some steps that must be done to finish the experiment. Such information is well known to the experienced researcher; however, Mark is just a first-year graduate student who doesn’t know what to do. He then finds the specific paper with our platform and tries to upload a question specifically denoting which part of the paper the question is about. He finds out that similar questions have already been asked by someone else, and use that as his answer. He gives a vote for the question and answer that helps him allowing other people to know that the annotation can be trusted. Meanwhile, he gets a notification that his another question he uploaded a few hours ago has been answered and goes to check it out.

*User’s perspective:*
Swena is a post doctor student in bioengineering department of MIT and is a specialist in her research area. She likes answering questions using our platform because it feels very good to be recognized by other people. While reading a new paper on NATURE, she sees jack’s question and answers it as best as she can. As she read further she sees some bad answers to a certain question and makes her own new answer. With each annotation, she gets points which is used to rank the user in order of how much help he or she has given. Swena is ranked in 3rd place for entire users and when she goes to conferences she is always recognized and thanked by other researchers for answering their questions.

#### Seven dimensions
* Motivation - Reputation system would be the best motivation factor for this system.
* Aggregation - Every annotation will be shown on the text. If they get too much down votes, remove them from the sight(not delete). This will allow each annotation and questions to be related to the text more intuitively, instead of just listing them.
* Crowd pool - Main users of this platform would be students, researchers, scholars, or other academic people who work with academic papers often.
* Quality control - Workers and requesters should be identified before he or she makes any requests or annotations. Each annotation may be evaluated using up and downvoting.
* Human skill - Workers must read the paper and understand it thoroughly.
* Process-order - requester uploads a question about a certain paper. Worker answers the questions. The worker then replies to the questions. The computer does nothing.
* Goal visibility - All.

>### Feedback Sharing Platform

#### Summary
This platform crowdsources people to aggregate readers’ personal feedbacks on each paper--what they liked and disliked--so that others can have a deeper understanding of the paper in various perspectives.

#### Scenario (organic workflow):
*User’s Perspective:*
Harry is a Korean undergraduate student at KAIST, majoring in Computer Science. This is the senior year for Harry, so he decided to participate in individual research in an HCI lab. As the first step to doing research, Harry is given five CHI papers to read in a week. Harry has never read an academic paper before, and he is not a native English speaker either. The amount of reading he has to do stresses him out. Using his dictionary, he has finished reading the first paper. Even after finishing the reading, he understands what the paper is talking about a word to word, but he has no idea of if this is a generally considered “good” paper or what kinds of issues are present in the paper. Feeling frustrated, he decides to ask his friends for help, but, unfortunately, nobody has read the paper. Instead, Tom recommends Harry this feedback sharing platform for academic papers. Harry enters the website. He sees a big search box in the center of the page, saying “Enter the title, author, ISBN, etc. of the work”. Below the search box is a list of academic categories that are expanded into subcategories on click and navigated to a page that lists all the papers under the subcategory. Harry types in the title of the paper he has just read and hits the search button. The results show the right paper, and Harry clicks to the link. On the new page, Harry sees a list of feedbacks from different people. Many people who have read the paper have shared their personal thoughts about the paper, what they liked about the paper, how they think the research can be improved, and so on. Harry feels enlightened with new insights from a variety of people. He now feels hopeful about reading the rest four papers with the help of this platform.

*Worker’s Perspective:*
Six years later, now Harry is a Ph.D. candidate in the HCI lab. He is now somewhat experienced with paper reading as he has read hundreds of papers. Harry feels comfortable with reading a paper and having his own thoughts on the paper. He also has enough paper datasets to base his evaluation on paper. For his research on crowdsourcing, as usual, he has read a new paper published in CHI 2016. Instead of doing nothing with his reading, he shares his thoughts on the platform so that he can get others’ feedbacks on his feedbacks and also so that he can help out other people having a hard time to understand academic papers just like himself six years ago. He also loves how writing this feedback on the platform organizes his thoughts more clearly. 

#### Seven dimensions
* Motivation - Reputation system would be the best motivation factor for this system.
* Aggregation - Individual reviews are not completely merged into one, but top rated reviews appear on the top.
* Crowd pool - Main users of this platform would be students, researchers, scholars, or other academic people who work with academic papers often.
* Quality control - Each review may be evaluated using up- and downvoting.
* Human skill - Workers must have read the paper at least once.
* Process-order - The system provides the basic information about academic papers and creates space for discussion for each paper. Workers leave their own feedbacks in the space provided by the system. Users read the feedbacks on the platform and get inspired.
* Goal visibility - Visible to all.

>### Question-and-answer platform

#### Summary
We suggest a question-and-answer web platform where users can ask questions arise from academic papers.
#### Scenario
*User’s perspective: *
John is an undergraduate student who took the crowdsourcing course. It was his first time to read papers, thus he had a lot of questions. He had no friends to answer the question since crowdsourcing is an unfamiliar field. He instead searched the internet and found nice-looking sites where students freely share questions about papers. He posted a question and got an answer in few seconds. It was super famous replier who has answered hundreds of questions. John was satisfied with the clear answer. He accepts the answer sending a thank-you message. He still uses the site when he got stuck while reading a paper. 

*Worker’s perspective: *
Jay is a graduate student who has been supervised by his intense instructor. He has read thousand of papers and now became a specialist of crowdsourcing. At the first time, he didn't know anything about reading academic papers. He had no ideas how to find the paper, what to read in the paper, and how to understand it. He also had numerous questions about the paper. He tried really hard to get the answer. After those painful experience, he didn’t want other people to suffer from the same difficulties. He decided to share his knowledge in the web platform. He entered the site and found thousand of questions were already registered. The questions were sorted by fields, references, authors, keywords, and published year. It was easy to find the questions he can answer. He found the question related to crowdsourcing papers then replied to it. His answer was liked by other workers, and soon accepted by the questioner. The icon representing his state changed, meaning that he got more reputation than before. He enjoyed it a lot and keep participating in the platform. He is now one of the most influential workers in the platform.

#### Seven dimensions
* Motivation - The platform is highly dependent on reputation. A worker who has replied neat answers will become well-known and reliable.
* Aggregation - The worker’s replies are sorted by the questions that users posted. It will be all shown based on the quality it has.
* Crowd pool - Anyone can contribute to the platform.
* Quality control - The main method of quality control is a voting system. Workers can evaluate others’ work by voting.
* Human skill - Reading and understanding academic papers are required, which computers can’t do.
* Process-order - Requestors upload a question, and workers answer the question. The computer does subtle tasks like sorting.
* Goal visibility - The goal is visible to any workers.