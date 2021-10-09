# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

# My rail cheatsheet
## Explore different rails app creation options:

`rails new --help`

## How to run rails server and view it in the browser:

`rake db:create:all` (1st command)
`rake db:migrate` (2nd command)
`rails s` (run rails server)
it will build WEBrick, which is slow btw and start on the localurl
you can change the url running `rails server -h` for more startup options

## Scaffolds X Generators:

Keep in mind that Scaffolds create a lot of code and some of that code isn't always needed.


`rails g scaffold Project title:string description:text percent_complete:decimal`

then:

`rake db:migrate`

now run the server with `rails s`, open the localhost and type `/projects` at the end of the URL.****

With this our Scaffold gave us full CRUD functionality. We already have a database functionality where we can create/edit/delete objects in it.

## Running Rails on sandbox mode:

Type the command `rails c --sandbox` to enter sandbox mode and ctrl+D to exit

## To open the **console**

Type in `rails c` to start and ctrl+D to exit

## To see the routes withing the application:

Type in `rails routes` and it will show a list of the different used routes. Note that the command `rake routes` was deprecated.
