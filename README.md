# bardibardi Fork of Ruby on Rails Tutorial: sample application

This is a fork of the sample application for
[*Ruby on Rails Tutorial: Learn Rails by Example*](http://railstutorial.org/)
by [Michael Hartl](http://michaelhartl.com/).

(using rvm on ubuntu 11.04)

(rvm current yields ruby-1.9.3-p194@rt2)

git clone git://github.com/bardibardi/sample_app_2nd_ed

cd sample_app_2nd_ed

bundle install --without production

mod +x $rvm_path/hooks/after_cd_bundler

bundle --binstubs=./bundler_stubs

rake db:migrate

rake db:test:prepare

rspec spec

rails server

in browser goto localhost:3000

