## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.
  GET - show a record from the database
  POST - create a record in the database
  PUT - update a record in the database
  DELETE - remove a record from database

2. What is Sinatra?
  a framework that starts a server, and makes it simple to manage routes

4. What is MVC?
  convention from rails that is a standard template for organizing web app paths

5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
  in some cases it's necessary so that files can find each other, otherwise it's to get ready for rails

6. What types of variables are accessible in our view templates without explicitly passing them?
  all the regular ruby variables

7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
  
  ```ruby
  get '/horses' do
    @count = 1
    erb :index, :locals => {"name" => "Mr. Ed"}
  end
  ```
8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed`?

9. What's the purpose of ERB?
  gives you the ability to perform and output, the output from ruby logic directly in an html view

10. Why do I need a development AND test database?
  when each test is run, the database needs to be created and destroyed, so that variations across databases don't interfere with the test's ability to pass

11. What's responsive design?
  screen design that takes into account displays on all screen sizes; from mobile to large desktop

12. What is CRUD and why is it important?
  Create 
  Read 
  Update
  Destroy 
  It's the basis of how the internet works, transferring and modifying packets of data

13. What does HTTP stand for? 
  Hyper_Text_Transfer_Protocol

14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
  <%= some.ruby(displayed_usually_a_variable) %>
  <% other.ruby(not_displayed_usually_the_logic) %>

15. What's an ORM?
  object relational mapping

16. What's the most commonly used ORM?
  c++

17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
  /tasks GET
  /tasks POST
  /tasks/new GET
  /tasks/:id GET
  /tasks PUT
  /tasks/:id/edit GET
  /tasks DELETE

18. What's a migration? 
  when you want to add a table to your database

19. When you create a migration, does it automatically modify your database?
  not if the tables already exist

20. How does a model relate to a database?
  It uses activerecord / sql to query the database and return desired values to the controller/view

21. What's the difference between agile workflow and waterfall method?
  waterfall is archaic, dumb old, and expensive
  agile, is iterative, flashy, flexible, and saves you money

22. What is the difference between `#new` and `#create`?
  new just instantiates a new database object, create instantiates and saves that object to the database
