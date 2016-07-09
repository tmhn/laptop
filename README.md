# Sparta Global Laptop Config

This script is designed to install and configure Sparta student and trainer macOS machines.

### Manual Steps to install

1. Initial macOS Setup Wizard (Laptop name, WiFi etc). Admin staff will provide the username and password to use when configuring this part.
2. Run install script: `cd ~; bash <(curl -s https://raw.githubusercontent.com/spartaglobal/laptop/master/mac)` 
3. Type the admin password.
4. Wait **Ages**!
5. Install XCode (via App Store)
6. Celebrate 🍻!

### What does it do?

The script is fairly complex, and configures student laptops for our training courses. In general, it:

* Installs XCode command line tools.
* Sets the desktop background and user avatar.
* Sets a faster key repeat rate.
* Downloads and installs Sparta fonts, and rebuilds the font cache.
* Downloads and applies the `SpartaPro.terminal` theme.
* Installs and configures [Homebrew](http://brew.sh/).
* Installs the following libraries and tools using homebrew:
    - openssl
    - libxml2
    - libyaml
    - ctags
    - git
    - vim
    - heroku-toolbelt
    - hub
    - imagemagick
    - curl
    - chromedriver
    - httpie
    - node
    - rbenv
    - ruby-build
    - rbenv-default-gems
    - postgres
    - redis
    - sqlite
    - mongodb
* Sets `mysql` to run at startup.
* Installs the following GUI applications using `brew cask`:
    - Virtualbox
    - Vagrant
    - Google Chrome
    - Firefox
    - Sublime Text 3
    - Java JDK
    - Atom
    - GitHub Desktop
    - Slack
* Configures rbenv to `install` `bundler`, `brice`, `gist`, `pry`, `pry-doc`, `awesome_print`, `specific_install` with every new ruby installation.
* Installs the latest ruby version available from rbenv, and sets it globally.
* Updates all system gems and configures bundler to use parallel installation.
* Updates NPM and Node.
* Installs sensible `.vimrc`, `.bash_profile`, `.irbrc`, `.gitconfig` and `.pryrc` dotfiles.
* Installs vim-plug and the Vim plugins listed in `.vimrc`.
* Installs the following apps to `/Applications`:
    - MySQL Workbench
    - MacDown
* Installs and unpacks JMeter into `~`.
* Removes all default items from the dock, switches on magnification and adds Google Chrome, Atom, Mail and Slack to the dock.
* Runs a macOS Software Update.
* Builds the `locate` database.
* Clones the Sparta Workstation VM into `~/sparta/workstation`, configures it and provisions the vagrant box.
* Shuts down the Vagrant Box and restarts the machine.

### Inspiration

Bits of this script were borrowed from all over the internet, but in particular:
* https://github.com/attack/laptop
* https://github.com/thoughtbot/laptop/


### Links for installation packages
1. [Chrome](https://www.google.com/chrome/browser/desktop/index.html)
2. [Firefox](https://www.mozilla.org/en-GB/firefox/new/)
3. [Slack](https://slack.com/downloads)
5. [Sublime Text 3](https://www.sublimetext.com/3)
6. [MacDown](http://macdown.uranusjr.com/)
7. [Atom](https://atom.io/)
8. [Vagrant](https://www.vagrantup.com/downloads.html)
9. [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
12. Install [Java DK](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
13. Install [MySQL Workbench](https://dev.mysql.com/downloads/workbench/)


