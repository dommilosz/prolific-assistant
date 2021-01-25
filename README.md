## Installation tutorial

The most important dependency for this project is the Node.js interpreter and the NPM-JS package manager. Before running these commands/scripts, first install Node.js and NPM-JS. You can get them from here: https://nodejs.org/en/download/, https://www.npmjs.com/get-npm.

In the project directory, you should run:

### `npm i` (if the dependencies are not installed globally)
This will install all the dependencies needed to run and build the project

### `npm run start`

Compiles the extension into `./build/unpacked` to be loaded into your broswer for development. The extension automatically reloads when you save changes to the code.

##### Load into Chrome

1. Open Chrome
2. Go to `chrome://extensions`
3. Turn on `Developer mode`
4. Click `Load unpacked`
5. Select folder `./build/unpacked`

##### Load into Firefox

1. Open Firefox
2. Go to `about:debugging`
3. Click `Load Temporary Add-on...`
4. Open `./build/unpacked/manifest.json`

### `npm run build` (Alternative build to .zip)

Compiles the extension and packages them into production ready zips at `./build/{target}-{version}.zip`. These zips can then be uploaded to their respective extension stores.

---

Documentation: https://github.com/kadauchi/webextension-create#webextension-create
