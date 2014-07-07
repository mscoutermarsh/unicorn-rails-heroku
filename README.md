unicorn-rails-heroku
====================

Example Rails app w/Unicorn on Heroku.

This requires that Postgres be installed on your local machine.

```
$ git clone https://github.com/mscoutermarsh/unicorn-rails-heroku.git
$ cd unicorn-rails-heroku
$ bundle install
$ bundle exec rake db:create
$ bundle exec rake db:migrate
$ bundle exec rails s
```

Next, to get it running on Heroku.
```
$ heroku create
$ heroku addons:add heroku-postgresql:dev
$ git push heroku master
$ heroku open
```

See ```config/unicorn.rb```, ```Procfile``` and ```Gemfile``` for unicorn setup.

done!

### Need Help?
Tweet [@mscccc](http://twitter.com/mscccc)
