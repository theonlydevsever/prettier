# @theonlydevsever/prettier

![publish](https://github.com/theonlydevsever/prettier/actions/workflows/publish.yml/badge.svg)
![tag](https://github.com/theonlydevsever/prettier/actions/workflows/tag.yml/badge.svg)

[Prettier](https://prettier.io/) configuration for [@theonlydevsever](https://github.com/theonlydevsever)

## Install

```
// using yarn
yarn add -D @theonlydevsever/prettier prettier

// using npm
npm install --save-dev @theonlydevsever/prettier prettier
```

## Usage

This configuration can be set up using the `package.json` or `prettier.config.js` file.  

### package.json
```json
{
  "name": "no-transitory",
  "version": "1.0.0",
  "author": "alexisonfire",
  "prettier": "@theonlydevsever/prettier",
  "dependencies": {
    "react": "^17.0.1"
  }
}
```

### prettier.config.js
```js
module.exports = {
    ...require("@theonlydevsever/prettier"),
    // The configuration can be extended when using a prettier.config.js file
    semi: false
};
```

## Ignoring Files
If you want prettier to ignore certain files, create a `.prettierignore` file in your project's root firectory and add all of the files you want prettier to ignore.  

Here is our recommended `.prettierignore` 

```
node_modules
public
provisions
coverage
build
docs
db
*.svg
*.DS_Store
*.md
*.d.ts
```