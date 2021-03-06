# Jungle

A mini e-commerce application built with Ruby (-v2.6.6) on Rails (-v4.2) as a student assignment for Lighhouse Labs full-stack web development program. TDD (test-driven development) practices are followed using RSpec library. Stripe platform is used for payments.

## Features
Admin users can list and create new categories

Admins can add new products using the new category

Visitors can go to the registration page from any page in order to create an account

Visitors can sign up for a user account with e-mail, password, first name and last name

Visitors can sign in using e-mail and password

Visitors can log out from any page

## Additional Steps for Apple M1 Machines

1. Make sure that you are runnning Ruby 2.6.6 (`ruby -v`)
1. Install ImageMagick `brew install imagemagick imagemagick@6 --build-from-source`
2. Remove Gemfile.lock
3. Replace Gemfile with version provided [here](https://gist.githubusercontent.com/FrancisBourgouin/831795ae12c4704687a0c2496d91a727/raw/ce8e2104f725f43e56650d404169c7b11c33a5c5/Gemfile)


![](https://github.com/Mahir45/Jungle-rails/blob/master/app/assets/images/Screen%20Shot%202022-01-13%20at%202.20.37%20PM.png?raw=true )

![](https://github.com/Mahir45/Jungle-rails/blob/master/app/assets/images/Screen%20Shot%202022-01-14%20at%2012.58.13%20AM.png?raw=true)

## Setup

1. Run `bundle install` to install dependencies
2. Create `config/database.yml` by copying `config/database.example.yml`
3. Create `config/secrets.yml` by copying `config/secrets.example.yml`
4. Run `bin/rake db:reset` to create, load and seed db
5. Create .env file based on .env.example
6. Sign up for a Stripe account
7. Put Stripe (test) keys into appropriate .env vars
8. Run `bin/rails s -b 0.0.0.0` to start the server

## Stripe Testing

Use Credit Card # 4111 1111 1111 1111 for testing success scenarios.

More information in their docs: <https://stripe.com/docs/testing#cards>

## Dependencies

* Rails 4.2 [Rails Guide](http://guides.rubyonrails.org/v4.2/)
* PostgreSQL 9.x
* Stripe
