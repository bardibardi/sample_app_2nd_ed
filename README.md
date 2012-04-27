# bardibardi Fork of the Ruby on Rails Tutorial: sample application

This is a fork of the sample application for
[*Ruby on Rails Tutorial: Learn Rails by Example*](http://railstutorial.org/)
by [Michael Hartl](http://michaelhartl.com/).

# GIT

Crude push

% git push --repo=git@github.com:bardibardi/sample\_app\_2nd\_ed.git

Configure remote repository as origin

% git remote add origin git@github.com:bardibardi/sample\_app\_2nd\_ed.git

After the following, **git push** pushes the master branch to origin

% git push -u origin master

# Installation

(using rvm on ubuntu 11.04)

(rvm current => ruby-1.9.3-p194@rt2)

Pull repository

% git clone git://github.com/bardibardi/sample\_app\_2nd\_ed

Go to app root

% cd sample\_app\_2nd\_ed

Production requires postgres for Heroku deployment

% bundle install --without production

Make bundler hook executable

% mod +x $rvm\_path/hooks/after\_cd\_bundler

In order to eliminate the need to run **bundle exec**

% bundle --binstubs=./bundler\_stubs

Create development db

% rake db:migrate

Create test db ?? unnecessary ?

% rake db:test:prepare

# Tests

Run rspec tests

% rspec spec

Run cucumber tests

% cucumber features

# Development Server

Run webrick

% rails server

# Browser

In browser goto

http://localhost:3000

