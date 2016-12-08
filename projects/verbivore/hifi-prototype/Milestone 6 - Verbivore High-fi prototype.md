Oisin Daly Kiær, Paul Grau, Yoo Jin Lim

## Final Project: High-fi Prototype
Learnersourcing Vocabulary Flashcards

### Project Summary

Verbivore is a vocabulary flashcard studying and -generation application that attempts to lessen the tedious busywork associated with flashcard creation, while also using the crowd-work of its users to iteratively improve its set of cards. Users study by themselves, while being confronted with microtasks that help them learn, while we use their tasks’ output to improve the cards themselves. Iterative improvement towards a set of ‘holy-grail’ perfect vocabulary flashcards.

### Instructions

To get started, you have to create a user (email and password--though we don’t send anything to the email address). Afterwards, it’s relatively straight-forward. Click on the ‘get started’ button, and we will select ten words for you to study. You study the card, and when you finish, you will be presented with a microtask related to the card. This can be something like rating the example sentences you have seen, or creating a new one.

If a feature is bad, you can flag it. Perhaps an example sentence uses the word wrong? You can mark that, and another user will be tasked with fixing it later. Work through some sets and see what you think! Remember that the tasks we give you are the main benefit of Verbivore. Doing the work forces your brain to understand the word much better than just reading it and moving on.

### Technical Description

The entity relationship diagram for the database looks like this.

![ER diagram sketch](image_0.png)

All user submissions are in the form of ‘Features’. A feature can contain multi-media content; text, image, sound (perhaps video in a future version). Verbivore does not do any hosting itself, but rather relies on an external hosting source (e.g imgur for images). A feature holds its text if that is its content, or the URL of its content if it is sound/video

#### Backend stack

The backend is written in Python, using Flask as the server framework and SQLAlchemy as an abstraction layer on top of a RDBMS (SQLite for local development, PostgreSQL for deployment). It contains the data structure of features, cards, tags, users, votes and microtask results, as well as an API that lets the frontend extract them as JSON objects. Additionally, we have a script here that scrapes words and definition from this URL to have some seed data: [https://raw.githubusercontent.com/yiransheng/Pervasive-GRE/master/dictionaries/gre.json](https://raw.githubusercontent.com/yiransheng/Pervasive-GRE/master/dictionaries/gre.json)

For each word, part of speech and example sentences are gathered from the Pearson Dictionary API, available at: 

[https://github.com/PearsonAPI/PearsonSDKDictionarySample](https://github.com/PearsonAPI/PearsonSDKDictionarySample) 

This forms the content base for our users to learn from working on microtasks. We have some concerns about this data set: The example sentences are of considerably high quality, generally. It’s currently non-trivial to make improvements to them. We may need to strip them down to introduce niches for our users to fill. Furthermore, the example sentences that we display on each showing of a card are picked here using random sampling. It’s done with a multi-armed-bandit-esque system: A feature’s votes translate to a probability, and we sample two sentences from the distribution over all the card’s features (Exploitation). We also take a third sample from a uniform distribution over the feature set, to give new features a chance to be seen (Exploration).

#### Frontend

The frontend is written in Javascript (ES6 using Babel). The UI is based on the React library and is designed after Google Material-UI conventions. Together with React, we use the Redux pattern, the two of them famously pairing quite well together, on account of their almost taoistic input/output symmetry. This was chosen based on the members’ familiarity and interest in learning the React-Redux framework. Paul and Yoo Jin were already familiar with it, and Oisin wanted to learn it. It also happens to work well with our application, and indeed most web-apps, with its heavily state-based design. The usage of React-Redux happens to be quite justified in our application. Google Material-UI is the fashion for UI design at the moment, making it a natural choice as our design components. Most users are familiar with the Material-UI pattern at this point.

#### Deployment

We used Heroku for a quick and easy deployment. It automatically builds both the backend and frontend and connects to a PostgreSQL database.

### Prototype URL

[http://app.verbivore.cat](http://app.verbivore.cat)

### Prototype Code

[http://github.com/graup/verbivore](http://github.com/graup/verbivore)

