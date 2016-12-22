## Week Three Recap

### Instructions
Fork this repository. Be sure to pull the latest changes to your local repo. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What is the entry at the command line to create a new rails app?
  rails new AppName -T --database=postgresql --skip-turbolinks --skip-spring
2. What do Models generally inherit from in rails?
  ActiveRecord::Base
3. What do Controllers generally inherit from in a rails project?
  ApplicationController
4. How would I create a route if I wanted to see a specific horse in my routes fitle assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?
  resources :horses, only: [:show]
5. What rake task is useful when looking at routes, and what information does it give you?
  rake routes: path, uri, controller#action
6. What is an example of a route helper? When would you use them?
  resources :horses, as: 'awesome_horses'
  if you had a normal resource of horses, that weren't awesome and you want an extra degree of separation between the two
7. What's the difference between what `_url` and `_path` return when combined with a routes prefix?
  path is relative, url is absolute
8. What are strong params and why are the necessary?
  it's how rails makes you import input from forms, helps with security, prevents malicious code from being input
9. What role does `form_for` play in helping us create our forms?
  it creates the form, and the path to which the data is sent
10. How does `form_for` know where to submit the user's input?
  some black magic (for edit v new), but you also define it in the first line
11. Create a form using a `form_for` helper to create a new `Horse`. 
  <%= form_for @horse do |f| %>
    <%= f.label :name %>
    <%= f.text_field :name %>

    <%= f.label :breed %>
    <%= f.text_field :breed %>

    <%= f.submit %>
  <% end %>
12. Why do we want to validate our models?
  so that incomplete entries are not saved to the database, or the information that the app needs to use actually gets saved
