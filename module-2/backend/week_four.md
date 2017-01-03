## Week Four Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

* What is a cookie?
  - information about the user that is stored in their browser
* What’s the difference between a session and a cookie?
  - sessions are stored for the duration of the current session (i.e. user id), cookies persist (i.e. preferred language = english)
* What’s a flash and when do you want to use flashes?
  - temporary message, notify user of login/logout/something crudded, etc. 
* Why do people say “HTTP is stateless”?
  - because when the server treats every request it receives the same, so you need to send information
    about the user's state so the server knows the appropriate way to handle the request
* What’s authentication? Explain.
  - making sure that the person who sends an http request is who they say they are, by making them login
* What’s the difference between authentication and authorization?
  - authorization limits what a user can see based on who they are, authentication checks that a user is who they say they are
* What’s a before filter?
  - a (helper?) method that is triggered before a controller method, ex. checks that a user is logged in before they can view 
    a certain page
* How do we keep track of a user once they’ve logged in?
  - store their information in the session
* When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?
  - for admin privileges
* At a high level, what tools can you use to implement authorization? How would you use them?
  - Oauth / facebook, google, twitter, etc. 
* What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?
* What are some strategies you can use to keep your views DRY?
  - partials
