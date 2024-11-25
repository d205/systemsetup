## Installing NVM

Prerequisites:

* Homebrew(refer to [Readme.md](./README.md))

Installation steps:

Once you have Homebrew installed, you can use it to install nvm by running the following command:

``brew install nvm``

Add nvm to your shell profile: TO make nvm available every time you open a new terminal window, you will need to add the following line to your shell profile (e.g., ~/.base_profile or ~/.zshrc or ~/.zprofile)

``source $(brew --prefix nvm)/nvm.sh``

Now check nvm is install 

``nvm --version``

## Install Node

Two ways:

1 Install latest version
``nvm install node``

2 Install lts version (recommended)
``nvm install --lts``

## How to set default version

``nvm alias default <version of node>`` for example ``nvm alias default 18``


