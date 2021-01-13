# THREADLY
Rails app for a commenting service

![app](https://user-images.githubusercontent.com/58056552/104485968-24c24200-5599-11eb-9b8e-ea50b76a5a4c.png)


### Key concepts
Use migrations to update columns in the database 	
~~~~
$ bundle exec rake db:migrate 
~~~~
Display data in the view
~~~~
$ bundle exec rake db:migrate 
~~~~
Utilize the form_for helper method
~~~~html
<ul class="comments">
  <% @all_posts.each do |p| %>
    <li><%= p.comment %></li>
  <% end %>
</ul>
~~~~
Use resources in the routes file 
~~~~ ruby
Rails.application.routes.draw do
  root "posts#index" 
  resources :posts
end
~~~~
watch the database

~~~~
$ rails c
$ Post.all 
~~~~
