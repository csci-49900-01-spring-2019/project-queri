# Queri Application
Web & Android Client for Queri Application.

## Content

### Abstract

Queri is an application where users can ask and answer questions. Users have the option to either stay public on be anonymous when asking and answering questions. Users can vote for their or other user's questions to be featured on the front page. The User can only vote for a question once and only once (there is no exception). Questions will cycle on the front page every 7 days so users will have enough time to answer questions if needed. Queri was made so users can ask any questions they have without being criticized or being biased and have a response to their answer.

### Introduction

Queri is a discussion tool where users can ask or answer questions with the option of staying public or anonymous. The objective is to eliminate any biased towards other users and have users ask questions without them having feeling safe. Users should not be afraid of asking a question just because their posts can be traced or found by another person. On Reddit, users can see the responses to a post without answering the post so their answers may get swayed. We want to prevent that as we want users to get personal responses not swayed by other user responses.

When a user asks or answers a question, they will have the option to stay anonymous or public. Other users will not be able to see other user's profile so users can feel safe when asking or answering questions and not have the fear of their posts being traced or found by another person. Users will also not be able to see other user's responses to a specific question without submitting a response of their own. This is to prevent users from getting their personal responses swayed because they saw another user's response. 

## Main Content

The idea of staying anonymous or public is a feature for users to have an option for more sense of security. Users should the option of submitting questions and answer anonymously or not as our objective was for users to not be afraid of asking or answering questions online. We also wanted to remove users being bias therefore users having the option to stay anonymous would remove any sort of users being bias. With the users being anonymous, we feel more questions will be asked as users won't have to worry about anything being revealed to other users. Our goal for our application was for users to ask questions and get their questions answered without them having to worry about other people criticizing them. We also didn't want users to post offensive responses to other user's questions so we wanted to implement a report button where if a post gets a certain amount of reports, it would be removed and deleted off our database. But because of our time constraint, we could not get to implement the report button into our application.

Our work is original with the anonymous feature. Our idea for this project is for users to ask and answer questions online while the option to stay anonymous or public to other users. Reddit has a similar structure to our idea where users can post but did not have an option to stay anonymous. Reddit is also a discussion tool so users can not only post questions but they can post information and etc. Our idea is for users to only post and answer questions online so users can have thier questions answered within a certain time frame. To let users see anything our application has to offer, they would need to register for an account otherwise they would not be able to use all of our features on our application. Once a user has made an account, they would not be able to see the responses of any questions unless they made a response of their own. We feel a person should not submit responses because of another user's response has swayed their response unlike Reddit where users can see responses even if they did not register for an account. Users can vote for questions to be featured on the home page and a total of 10 questions will be shown in a certain time frame using CronJob. Once the time frame has expired the questions will be sent to archive where users will no longer be able to post responses. 

We wanted to have an algorithm where users can only post a specific amount of characters when submitting a question or comment. We also decided to use Angular 7 as our web development platform and Android Studios with our android development platform. As we progressed on using Angular 7, we encountered many issues and felt like the learning curve was steep. With Angular 7, we had to use typescript and many of us were more familiar with javascript. Although typescript is similar to javascript, we still struggled with learning the platform. With Android Studios, we used Java and as said previously, some of us had previous experience with Android Studios and Android 
Studios uses Java. For data, we have three nodes, which are voting, archive and featured. Each question has a random generated id attached and the three nodes have the same structure so because they have the same structure, we can make the same API call to call them. 

We fulfilled the web service requirement by using heroku. Our application was deployed on the [server](queri499.herokuapp.com) and is working correctly. When we deployed our application to heroku at first, we encountered some issues. One of the issue was our package.json file was encountering some issues as we did not know that there was a command for devDependencies to be used. Our first solution was to move all the devDependencies to the Dependencies in the package.json file but that seemed rather insufficient so we found a command to input so devDependencies could be used on heroku. Once our application deployed to heroku, everything worked as intended and we did not run into further issues. The reason why we decided to use heroku as our web service requirement is because it was free so we didn't have to pay to have our application to be deployed. The other reason why we decided to use heroku was because it was rather simple to deploy our application to their server. It was easy to find fixes if we encountered any issues when deploying and we also got recommended to use heroku by peers. The only con of using heroku is that there is a data limit for their git remote repository but the service was free. Overall, we would recommend anyone to use heroku if you need a free service to deploy your application. 

We fulfilled the multiple native client requirement with Angular 7 and Android Studios. With Angular 7, we developed our web application. We connected our database, which is firebase, to Angular 7. With Angular 7, it was very easy to connect it with firebase and we had almost no troubles at all. The problem with using firebase with Angular 7, when we made our login component and made the user register for an account, they would get sent an email verification link through firebase but for some reason, firebase would send the email verification link very slowly. This is extremely bad for when users get very impatient and decide to keep clicking the resend email verification link and it gets sent very slow as when the user actually receives the email verification link, it would become invalid as the user click on the resend email verification link button too many times. Overall, we struggled a lot with making the web application because of how complicated Angular 7 was. With Android Studios, we developed our android application. We did not deploy this application anywhere as it was not a requirement. We did not have many issues with our android development as there were some people in our group that was familiar with developing android applications with Android Studios. The biggest issue we had with our android application was connecting firebase to Android Studios. Overall we struggled a bit with making the android application but most of the issues were easily fixed.

We fulfilled the security requirements for the web application with a email verification when a user signs up. When a user enters our application, they will have to register for an account. Once the user goes into the registration page, they will have the option to either register with an email/password OR they will have the option to register with the google authenication service. When the user signs up with email/password, they will be sent an email verification link. The user will not be able to log in until the user click on their email verification link. The problem with this security is that we are sending an email verification link with firebase so the email verification link can be sent to user's emails very slowly as we encountered this issue. When a user registers using the google authenication service, they will automatically be verified and will be able to log in right away and use all the features of our application. We could not figure out a way to make it so when the user signs up with the google authenication service, they will get an email verification link. The user will automatically be verified with the google authenication service. 

## Conclusion

For the web application, we have struggled with using Angular 7. Angular 7 had a huge learning curve that our group had to learn through. With the huge learning curve of Angular 7, we struggled with many things to develop our web application such as creating a custom username for users. For this android application, we encountered some issues but some of us had experience in making an android application before and was familar with the tools we were using. So we did not encountered as much issues with the android application.  We also learned how to work with a group as many of us did not ever code in a group before. We learned that time management is very important in a group and that communication is key to success in a group. 


## Authors

Web Development
* Angel Checo
* Kevin Yang
* Ramela Ramnauth

Android Development
* Svetleen Guerrier

## References

### Technology Used

* [Node JS](https://nodejs.org/en/)
  * [Express JS](https://expressjs.com/)
  * [Javascript](https://www.javascript.com/)
* [Angular 7](https://angular.io/)
  * [Typescript](https://www.typescriptlang.org/)
  * [Bootstrap](https://getbootstrap.com/)
* [Firebase](https://firebase.google.com/)
* [Android Studios](https://developer.android.com/studio)
  * [Java](https://www.java.com/en/)
* [Heroku](https://www.heroku.com)
  
  ## API Documentation
  
  Please refer to the Appendix to view our API Documentation or click [here](Appendix/DOCUMENTATION)
  
  ## Web Server
  If your interested in trying our application please follow the following instructions or visit our [website](queri499.herokuapp.com)
  
  ## Google Slides
  Our presentation slides can be found [here](https://docs.google.com/presentation/d/15MtLGrTOnDdzO2ulvzZPYesr4ojI3RM368-6TI3KpYw/edit?usp=sharing)
  
  ## Contact Us
  For any further questions or comments please contact us at projectqueri499@gmail.com
  
  
