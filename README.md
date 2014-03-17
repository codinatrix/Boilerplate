# Rails Boilerplate

This is a boilerplate startup app with all the gems and configs that I tend to use in every project. This is probably not
useful to anyone other than me.


Gems



* Postgres (because Heroku demands it)

* rails_12factor, rails3_serve_static_assets, rails_log_stdout for Heroku assets

* Memcachier, Dalli for performance on Heroku

* New Relic

* Rollbar error tracking

* Rack timeout to prevent hanging

* Unicorn in production only


Assets

* Twitter Bootstrap from CDN

* JQuery from CDN

* Placeholder.js from CDN

Make sure to set username and password in config/database.yml if not using Heroku. Heroku will automatically rewrite that file, so no 
worries with Heroku.

Run ```rake secret``` and copy the result into ```heroku config:set SECRET_TOKEN=something```. Do not commit that file publicly. 

```heroku create myapp``` and then you can push!
