##Creating a basic Ruby scripting template with RSpec:

Create directory with Gemfile, lib/, README.md and [.gitignore]("https://github.com/github/gitignore/blob/master/Ruby.gitignore")

Note that if you clone this directory you will need to delete .git/


### Set up version control:
Create a new repository on [Github]("https://github.com/") 

```
git init
git remote add origin git@github.com:scripttease/script_and_spec_template.git
git add --all
git push -u origin master
```


Set up Rspec:

```
rspec --init
```

Create _spec.rb files for each .rb file and require them by using this code
at the beginning of each _spec file:

```
#!/usr/bin/env ruby
require 'rspec'
require_relative '../lib/my_file'
```

Install dependencies:

```sh
gem install bundler
bundle install
```

Configure environment:

Add the following to each .rb file (top)

```ruby
#!/usr/bin/env ruby
```

Outline any usage instructions in the README.md:

```md
##Usage:

Install dependencies:
```

```sh
gem install bundler
bundle install
```

