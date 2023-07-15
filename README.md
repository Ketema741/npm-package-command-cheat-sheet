# npm-package-command-cheat-sheet

This cheat sheet provides a quick reference for commonly used npm commands.

## Getting Started

- Check npm version: `npm -v` (or `npm --version`)
- Get help: `npm help` or simply `npm`

## Creating and Configuring Packages

- Initialize package.json: `npm init`
- Initialize package.json with default values: `npm init -y` (or `npm init --yes`)
- Set default author name: `npm config set init-author-name "YOUR NAME"`
- Set default license: `npm set init-license "MIT"`
- Get default author name: `npm config get init-author-name`
- Get default license: `npm get init-license`
- Remove default author name: `npm config delete init-author-name`
- Remove default license: `npm delete init-license`

## Managing Packages

- Install local packages and save to dependencies:
  - `npm install lodash --save` (or `npm install --save lodash`)
- Install multiple local packages and save to devDependencies:
  - `npm install gulp gulp-sass --save-dev`
- Move to another folder and install dependencies: `npm install`
- Move to another folder and install only production dependencies: `npm install --production`
- Uninstall local package and remove from devDependencies:
  - `npm uninstall gulp-sass --save-dev` (or `npm remove gulp --save-dev`)
- Install specific package version: `npm install lodash@4.17.3 --save`
- Update package to the latest version: `npm update lodash --save`
- Install global modules: `npm install -g nodemon` or `npm install -g live-server`
- Run nodemon: `nodemon`
- Find root folder: `npm root -g`
- Remove global packages: `npm remove -g nodemon`
- List installed packages:
  - `npm list`
  - `npm list --depth 0` (shows top-level packages only)
  - `npm list --depth 1` (shows packages up to a depth of 1)
- Install live-server locally and save to devDependencies: `npm install live-server --save-dev`

## NPM Scripts

You can define custom scripts in the "scripts" section of package.json.

Example:

```json
"scripts": {
  "start": "node index.js",
  "dev": "live-server"
}
