## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR. 

1. At a high level, what is ActiveRecord? What does it do/allow you to do?
  - it is a bridge between your ruby code and the sql database
2. What kind of methods are `belongs_to`, and `has_many`? (i.e. class or instance) Give an example.
    class - they apply to every instance in that class
3. What do they allow you to do?
  allow you to define 1-m, 1-1, m-m, relationships between tables
4. What's the difference between agile workflow and waterfall method?
  agile - go step by step, heavy focus on refactoring at the end of each step and making sure that the endgame is still relevant/appropriate
  waterfall - define objective at beginning, go headstrong through scheduled set of steps and hope that by the end of the project the endgame is still appropriate
5. What is the difference between `#new` and `#create`?
  new doesn't save to database, create does
6. At a basic level, what does cURL allow you to do?
  trigger a browser request from terminal
7. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.
  many students to one teacher . . . a student only has one teacher, a teacher has many students
    students          teachers
    id                id
    name              name
    teacher_id
    
8. Define foreign key, primary key, and schema.
  foreign_key - points from a many to the one
  primary_key - unique identifier for each entry in a table, used in conjunction with foreign keys
  schema - overall database structure
9. Describe the relationship between a foreign key on one table and a primary key on another table.
  they are the same number, the foreign matches whatever primary key it wants to relate to
10. What are the parts of an HTTP response?
  headers - verb, path, protocol, a few other things
  body - optional content
11. Describe some techniques to make our Sinatra code more DRY. Give an example of when you would use these techniques.
  crudding, is basically a lot of copy and paste, use partials to minimize repeating yourself


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
4. What can you expect from a group as you begin working together? As you continue working together?
5. What two columns does `t.timestamps null: false` create in our database?
  created_at, updated_at
6. What cURL flag can you use to send a `POST` request?
7. What case does JSON (and JavaScript) use for multi-word variables?
8. What case does Ruby use for multi-word variables?
9. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
10. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
11. Give an example of when you might want to store information besides ids on a join table.
12. Describe and diagram the relationship between patients and doctors.
13. Describe and diagram the relationship between museums and original_paintings.
14. What are some examples of acceptable values for the parts of an HTTP response?
15. What types of output do we want to test when we test our controllers?
16. What could you see in your code that would make you think you might want to create a partial?
17. Why might you use a helper method?
