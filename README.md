# npm-package-command-cheat-sheet
npm -v (or --version)

# GET HELP
npm help
npm

# CREATE PACKAGE.JSON
npm init
npm init -y (or --yes)

# SET DEFAULTS
npm config set init-author-name "YOUR NAME"
npm set init-license "MIT"

# GET DEFAULTS
npm config get init-author-name
npm get init-license

# REMOVE DEFAULTS
npm config delete init-author-name
npm delete init-license

# INSTALLING LOCAL PACKAGES
npm install lodash --save (or npm install --save lodash)
npm install moment --save
npm install gulp gulp-sass --save-dev

# MOVE TO ANOTHER FOLDER
npm install
npm install --production

# REMOVING MODULES
npm uninstall gulp-sass --save-dev
npm remove gulp --save-dev

#INSTALL CERTAIN VERSIONS
npm install lodash@4.17.3 --save

# UPDATE
npm update lodash --save

# INSTALL GLOBAL MODULE
npm install -g nodemon
npm install -g live-server

# RUN NODEMON
nodemon

# FIND ROOT FOLDER
npm root -g

# REMOVE GLOBAL PACKAGES
npm remove -g nodemon

# LISTING PACKAGES
npm list
npm list --depth 0
npm list --depth 1

# INSTALL LIVE-SERVER LOCALLY
npm install live-server --save-dev

# NPM SCRIPT
"scripts": {
    "start": "node index.js",
    "dev": "live-server"
  },
