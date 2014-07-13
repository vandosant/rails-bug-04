# Rails Bug 04

## Setup

* `bundle`
* `rake db:create db:migrate db:seed`
* `rails s`

You can run specs with:

* `rspec`

Note: email/password combinations for existing users populated by `rake db:seed` can be found in the db/seeds.rb file.

## Stories

**Task creation can blow up (bug)**
```
As a user
When I go to add a task
And I forget to add a description
And I press create
Then I should see a validation error
But instead it blows up
```

## Wireframes

New task page w/ errors:

<img src="project/03-new-with-errors.png">
