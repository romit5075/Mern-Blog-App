# Blog.it

  <img src=/frontend/public/android-chrome-192x192.png>

A MERN stack blogging PWA(Progressive Web App), with user authentication and social login using Twitter and Google accounts.


## Getting Started

-   Fork this repo and run the `git clone <forked repo>` command from your terminal/bash
-   Cd into the directories and `npm install`
-   Create a `.env` file in the root directory and store the following:
    -   MONGO_URI=Insert the correct connection URL for your MongoDB database
    -   REACT_APP_GOOGLE_CLIENT_ID=Insert the valid google client id
    -   REACT_APP_TWIITER_CONSUMER_ID=Insert the valid twitter consumer id
    -   REACT_APP_TWITTER_CONSUMER_SECRET=Insert the valid twitter consumer id
-   Run the server on PORT 5000
-   npm start/yarn start

You can obtain the MONGO_URI after create a collectoin on [mongodb atlas](https://www.mongodb.com/cloud/atlas). For the GOOGLE_CLIENT_ID and the TWITTER_CONSUMER_SECRET/ID, you will need to go through the Google developer console and the Twitter developer accounts page respectively

## Demo

<p align="center">

 <img alt="login page" src="https://i.ibb.co/bWBJLhB/Screenshot-834.png" width="534" height="300" />
 <img src="https://i.ibb.co/4sHTB83/Screenshot-835.png" alt="home page" width="534" height="300" />
 <img src="https://i.ibb.co/jg6rXpx/Screenshot-836.png" alt="rich editor" width="534" height="300" />
 <br/>
  <img alt="mobile mockup" src="https://i.ibb.co/ZK3VRNF/mern-blog-it-herokuapp-com-Moto-G4-2.png" width="200" height="356"/> &emsp;
  <img alt="mobile mockup 2" src="https://i.ibb.co/1TkMF7Q/mern-blog-it-herokuapp-com-Moto-G4-1.png" height="356" width="200" />
  <br/>
  <img alt="tablet mockup" src="https://i.ibb.co/bKqyx4w/mern-blog-it-herokuapp-com-i-Pad-1.png" width="300" height="402"/> &emsp;
  <img alt="tablet mockup 2" src="https://i.ibb.co/vVNQ61w/mern-blog-it-herokuapp-com-i-Pad.png" width="300" height="402"/>
  
</p>

## Info

-   This is a blogging PWA with user authentication and authorization. There is also a social login option, to login using your Twitter or Google accounts. The blog posts are displayed in the reverse chronological order by default.
-   There is no exploitation of data, as the app only requires access to your accounts to fetch your unique ID for authentication/authorization purposes, and no personal details(except your registred user name on the social account) is used by the application.
-   The frontend of the app is built using React and I have used Bootstrap classes for styling the compnents in addition to my local CSS styles.
-   It is a blog app that lets users read the existing blog posts without logging in, and lets them share their thoughts using the anonymous comment section.
-   Each comment has a unique jdenticon icon to represent the user who commented anonymously
-   There is also a profanity filter to disallow usage of certain NSFW words in the comments' section. This is not an attempt to hinder freedom of speech, but instead it is a necessary aid to prevent misuse of the platform by nefarious users.
-   In order to write a new blog post, the user has to login using one of the social media login options provided. The react-social-login package is being used to provide the user authentication and authorization.
-   It has been deployed using Heroku's free tier and the Mongodb Atlas's cloud service is used for the database service. The access to the database is restricted to only 1 authorised user, and as mentioned earlier, there is no personal user data stored in it.
-   The rich editor used is the CKEditor 5's React WYSIWYG component (What You See Is What You Get) with a toolkit that supports bold, italics, hyperlinks, image embeds, indentations, blockquotes, video embeds, lists (ordered and unordered) and options to undo and redo changes as needed.
-   The application currently has more then 60 registered users, you can check out the app [here](https://mern-blog-it.herokuapp.com/) or by using the link in the description section


## Potential Improvements

-   A UX refactor.
-   Dashboard implementation for all registered users.
-   More social login options including the likes of Github, Facebook, Amazon or Apple.
-   Fuzzy Search implementation.
-   Integrations with popular blogging platforms like Medium or dev.to, to import already published articles.
-   A system to 'like' or upvote potentially useful articles.

Any more suggestions are always welcome in the PRs!

## Technologies Used

Some of the technologies used in the development of this web application are as follow:

-   [MongoDB Atlas](https://www.mongodb.com/cloud/atlas): It provides a free cloud service to store MongoDB collections.
-   [React.js](https://reactjs.org/): A JavaScript library for building user interfaces.
-   [Node.js](https://nodejs.org/en/): A runtime environment to help build fast server applications using JS.
-   [Express.js](https://expressjs.com/): A popular Node.js framework to build scalable server-side for web applications.
-   [Mongoose](https://mongoosejs.com/): An ODM(Object Data Modelling)library for MongoDB and Node.js
-   [Heroku](http://heroku.com/): A platform(PaaS) to deploy full stack web applications for free.
-   [JSON Web Tokens or JWTs](https://jwt.io/): A standard to securely authenticate HTTP requests
-   [Bootstrap 4](https://getbootstrap.com/docs/4.0/getting-started/introduction/): A popular framework for building responsive, mobile-first sites.

It can be noted that React can be swapped out in favor of any other popular frontend framework like Vue, Angular, Svelte or Ember. The server side can be implemented using Deno/Koa, flask/Django and similarly the data can also be modelled using the similar idea but with a SQL type DB like PS-SQL or MSSQL.
