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


https://www.pluralsight.com/guides/ruby-ruby-on-rails/token-based-authentication-with-ruby-on-rails-5-api

rails s
rails c
User.create!(email: 'example@mail.com' , password: '123123123' , password_confirmation: '123123123')
Item.create!(name: 'first item' , description: 'the first item is the first item')

curl -H "Content-Type: application/json" -X POST -d '{"email":"example@mail.com","password":"123123123"}' http://localhost:3000/authenticate

curl -H "Authorization: eyJhbGciOiJIUzI1NiJ9.eyJ1c2VyX2lkIjoxLCJleHAiOjE1MTg3Mjc5ODB9.FZ7s9I2WxjJiWwZyO4bzrhxumYWqKROckv2y_ieFA" http://localhost:3000/items