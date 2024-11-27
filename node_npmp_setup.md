# Node and NPM setup

## 🪜 Steps 
1. Install NVM
  * ``brew install nvm``. Follow detailed installation steps [here](./nvm.md)
  * Install latest node lts version


## How to manage two npmrc globally

### 1. Install npmrc
To install npmrc, on the command line, run ``npm i npmrc -g``

### 2. Create your first npm profile
After installing npmrc, you can create a profile to access your custom (maybe company's) registry.

To create an npm Enterprise profile, on the command line, run ``npmrc -c name-of-profile``. For example, to create a profile called "work", run the following command: ``npmrc -c work``

To set an npm Enterprise registry for the profile, run the following command, replacing ``your-company-registry`` with the name of your company's npm Enterprise registry:

``npm config set registry https://registry.your-company-registry.npme.io/``

### 3. Create a profile for the public npm registry
After you have created your npm Enterprise profile, you can create a second profile for a different registry, such as the public npm registry.

To create a profile for the public registry, on the command line, ``run npmrc -c name-of-profile``. For example, to create a profile called "open-source", ``run npmrc -c open-source``. To set the public registry for your open source profile, run the following command: ``npm config set registry https://registry.npmjs.org/``

### 4. Switch profiles with npmrc
To switch profiles, on the command line, run the following command, replacing profile-name with the name of your profile:

``npmrc profile-name``
