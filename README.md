# Heroku buildpack for running rake db migration on deploy

This buildpack is intended for use after the regular [ruby-buildpack].

# Usage

If you are using the default buildpack, manually set your buildpack to Heroku's default Ruby buidlpack

```
heroku buildpacks:set https://github.com/heroku/heroku-buildpack-ruby
```

Append the buildpack-ruby-rake-db-migrate to your buildpack list:

```
heroku buildpacks:add https://github.com/kespry/buildpack-ruby-rake-db-migrate
```

You are all set! Now whenever a deployment happens, the db will be migrated automatically during the deploy.

# License

MIT, see the LICENSE file.

[ruby-buildpack]:https://github.com/heroku/heroku-buildpack-ruby
