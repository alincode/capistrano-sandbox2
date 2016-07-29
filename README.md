# capistrano-sandbox

[capistrano website](https://github.com/capistrano/capistrano)

### create config

```
touch Gemfile
```

Install Capistrano, cap install STAGES=staging,production

`cap install`

or

`bundle exec cap install STAGES=local,sandbox,qa,production`

## Command-line usage

```
# list all available tasks
$ bundle exec cap -T

# deploy to the staging environment
$ bundle exec cap staging deploy

# deploy to the production environment
$ bundle exec cap production deploy

# simulate deploying to the production environment
# does not actually do anything
$ bundle exec cap production deploy --dry-run

# list task dependencies
$ bundle exec cap production deploy --prereqs

# trace through task invocations
$ bundle exec cap production deploy --trace

# lists all config variable before deployment tasks
$ bundle exec cap production deploy --print-config-variables
```

### reference
[Capistrano 自動化部署](http://xtony77.logdown.com/posts/210310-notes-capistrano-rails-deployment-automation)
