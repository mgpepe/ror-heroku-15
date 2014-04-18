INSTALLING ROR locally and on heroku in 15 minutes
==================================================

> 1. OSX only
> 2. If you have better/faster ways, let me know



Install Homebrew

    ruby -e "$(curl -fsSL https://raw.github.com/mxcl/homebrew/go)"

Remove RVM if exists because it is not compatible with rbenv

    rvm implode
    sudo rm /etc/rvmrc
    rm ~/.rvmrc

Install rbenv and ruby-build

    brew update
    brew install rbenv
    brew install ruby-build
    
Install ruby (rubyonrails.org currently recommends 2.1.0)

    rbenv install 2.1.0
    rbenv local 2.1.0
    echo 'eval "$(rbenv init -)"' >> ~/.bash_profile
    
Check version with:

    ruby -v
    
The run:

    sudo gem install bundler
    rbenv rehash

Install rails

    mkdir project_folder
    cd project_folder
    gem install rails
    
