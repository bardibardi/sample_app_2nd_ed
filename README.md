# bardibardi Fork of Ruby on Rails Tutorial: sample application

This is a fork of the sample application for
[*Ruby on Rails Tutorial: Learn Rails by Example*](http://railstutorial.org/)
by [Michael Hartl](http://michaelhartl.com/).

(git push --repo=git@github.com:bardibardi/sample\_app\_2nd\_ed.git)
(git remote add origin git@github.com:bardibardi/sample\_app\_2nd\_ed.git)
(git push -u origin master)

(using rvm on ubuntu 11.04)

(rvm current yields ruby-1.9.3-p194@rt2)

git clone git://github.com/bardibardi/sample\_app\_2nd\_ed

cd sample\_app\_2nd\_ed

bundle install --without production

mod +x $rvm\_path/hooks/after\_cd\_bundler

bundle --binstubs=./bundler\_stubs

rake db:migrate

rake db:test:prepare

rspec spec

rails server

in browser goto localhost:3000

