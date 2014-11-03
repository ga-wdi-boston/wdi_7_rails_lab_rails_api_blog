# Rails API blog lab

### Instructions

Clone this repo:
- `git@github.com:ga-wdi-boston/wdi_7_rails_lab_rails_api_blog.git`

Create a new Rails API application in this directory
- `rails-api new . blogAPILab --database=postgresql -T`

Scaffold Posts and Comments
- `rails g scaffold Post title body:text`
- `rails g scaffold Comment content post:belongs_to`

Setup associations between Posts and Comments in the models

Create a new Heroku app and push to Heroku
- `git add .`
- `git commit -m "Created new app with posts and comments"`
- `heroku create`
- `git push heroku master`
- `heroku run rake db:migrate`
- `heroku open`

Watch the [Railscast on Rails API](http://railscasts.com/episodes/348-the-rails-api-gem).
Read the [rails-api documentation](https://github.com/rails-api/rails-api).

Setup routes and controller so that comments are nested under posts.

Read on [Active Model Serializers](https://github.com/rails-api/active_model_serializers).
Watch the Railscast on [Active Model Serializers](http://railscasts.com/episodes/409-active-model-serializers).

Read on [jBuilder](https://github.com/rails/jbuilder).
Watch the Railscast on [JBuilder](http://railscasts.com/episodes/320-jbuilder).

What are the differences between Active Model Serializers and JBuilder? When might you use them?

Use JBuilder to make a serializer that returns all of the comments with each post.
