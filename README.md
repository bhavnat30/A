# README

Step1: Download Ruby on your local machine or use AWS Cloud 9 as it provides Ruby on Rails development Support. Follow the link for installing and setting up Ruby on Rails on windows machine:
https://gorails.com/setup/windows/10

Step 2 :Download and Extract the Code

Step 3: ecomApp folder 

Step 4: Install dependenices using the following Command:
bundle install

Step 5: Open the development.rb file located in config->environments folder and Add the corresponding content
in a single line! to the development.rb file
 FOR LOCALHOST: 
config.action_mailer.default_url_options = { host: 'localhost',port: 3000 }
For  Cloud9:
config.action_mailer.default_url_options = { host: ENV['IP'],port: ENV['PORT'] }

Step 6: Start Rails server using the command :
rails s

Heroku deployment steps:

Step 1:(Assuming you have heroku and git cli installed)
git init

Step 2:
heroku login -i

step 3:
git add .

step 4:
git commit -m "My first ROR application"

Step 5:
heroku create 

Step 6:
git push heroku master
