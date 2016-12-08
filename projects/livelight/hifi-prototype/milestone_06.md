# Milestone 6 - High-Fi Prototype

## Project Summary

Generating highlights for live videos such as sports match, presidential debates etc. needs experts and also viewers might have to wait for some time in order to watch those highlights.

We present LiveLight which uses every viewer's individual moments (moments they love) to generate highlights during the live stream.
 
As far as we know, our proposed system is first of its kind that uses crowdsourcing for highlight generation. The unique feature of our system is that it processes crowd's moments during the live stream and generates highlights before the live stream ends.

## Instruction

1. At first all user must be signed up to use our system.
<img src = "https://s3.ap-northeast-2.amazonaws.com/kaist-cs492-livelight/screenshot_06_01.png" width = 500>

1. After logged in, user can use our system.
<img src = "https://s3.ap-northeast-2.amazonaws.com/kaist-cs492-livelight/screenshot_06_02.png" width = 500>

1. There are three main components in our interface.
	* **Video Player**
		* Our video replays after every one hour.
	* 	**"Add This Moment!" Button**
		* User press this button when they found the interesting moment of the video.
		* User can cancel their miss response by clicking **undo button** on the left.
	* **List of Highlights**
		* Dynamically generated highlights (by the system based on users clicked data) will be listed on the right side of the page.


## Technical Description

### Frameworks

Livelight is implemented using **node.js v6.6.0** as a serverside framework and bootstrap **Bootstrap v3.3.7** as a front-end web page development.

### Libraries

To make the system look better, we used **Bootflat v2.0.4** css skins along with BootStrap.

The interaction between the server and client is done two ways: 1) Ajax(Asynchronous JavaScript and XML), 2) WebSocket. In order to handle Ajax Restful APIs on front-end, we used **JQuery v3.1.1**. In order to handle socket-based communication, we used **socket.io v1.4.5**.

In order to show videos, we used **video.js v4.3.0**, and used extensions like **videojs-markers v0.6.1** and **videojs.disableProgress**. Also, we did customization on the css to make it more suitable for our purpose.

For mongoDB ODM, we used **mongoose v4.4**. 

Also, we generate thumbnail images with **html2canvas v0.5.0-beta3**.

Finally, the authentication of users is done with **passport v0.1.18**.

### Technical Stack

The server is running on **Heroku**(https://www.heroku.com/), which is a platform-as-a-service(PaaS). We used hobby($7) sized instance for our system. As Heroku nicely supports scaling the system, we can handle the scalability issue pretty easily. 

mongoDB is running on **mLab**(https://mlab.com/), which is a mongoDB platform that hosts mongoDB.

On top of above infrastructure, we run our node.js express server and bootstrap & jQuery based front-end.

## Prototype URL

You can use our prototype here: https://live-light.herokuapp.com/

## Prototype Code

The repository of Livelight is available at https://gitlab.com/CS492/term_project.git
