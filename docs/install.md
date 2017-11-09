## Set Up Instructions

These instructions mostly follow the set up for the [Scotch.io Jekyll tutorial](https://scotch.io/tutorials/getting-started-with-jekyll-plus-a-free-bootstrap-3-starter-theme).

Install Xcode command line tools, homebrew, Ruby, RubyGems, Node.js, Bundler, and Jekyll.

```
# Xcode CLT
$ xcode-select --install
# Homebrew. Skip if you already have this installed.
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew doctor
$ brew update
# Ruby
# brew install rbenv ruby-build
$ rbenv install 2.2.2
$ rbenv global 2.2.2
$ ruby -v
# Optional: Add rbenv to bash so that it loads every time you open a terminal
$ echo 'if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi' >> ~/.bash_profile
$ source ~/.bash_profile
# Check that RubyGems was installed correctly
$ gem -v
# Update RubyGems
$ sudo gem update --system
# Bundler
$ sudo gem install bundler
$ brew install node
# Jekyll
$ gem install jekyll
$ jekyll -v
```
