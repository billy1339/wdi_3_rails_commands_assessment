# Rails Commands Quiz

Fork, clone, and write your answers directly in this file. Then submit a pull request.

### Question 1

I want to start a new Rails project/app called `BunnyApp`. What command should I type in the terminal?

rails new BunnyApp --database=postgresql

<!-- next time put a -T at the end -->

### Question 2

I want to create a new model called `Bunny`, with the following attributes: name (string), color (string), and age (integer). What command should I type in the terminal?

rails g model Bunny name color age:integer

### Question 3

What does the command in Question 2 do, exactly? What files are created, where are they located, and what does the database look like at this time? Explain.

rails g model: creates a file app/models/bunny.rb which defines the Bunny as a Ruby class, AND creates a migration file in /db/migrate with the columns and datatypes that were specified in the Terminal command

the command in Q2 creates 3 files  for name color and age within the models folder which is within the app folder

### Question 4

I want to create a database and make it reflect the new model I created in Question 2. What command(s) should I type in the terminal?

rake create:db -- this will create the database

<!-- rake db:create db:migrate
or  rake db:create
    rake db:migrate
 -->


### Question 5

I want to look at the actual database that has been created. What command should I type in the terminal?

rails db

### Question 6

I want to see a list of all the URLs available in my app, along with the HTTP requests and controllers associated with them. What command should I type in the terminal?

rake routes

### Question 7

I have worked on my app and finally want to see it in action. What command should I type in the terminal, and where should I navigate to in my browser?
terminal: rails s
browser: locakhost:3000/bunnys
