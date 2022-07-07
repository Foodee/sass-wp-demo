# sass-wp-demo
Demos how to namespace Wordpress css using SASS

## Installation
This demo requires NPM. On mac, you can install NPM using `brew`

```
brew install node
```

Once installed, you need to initialize the project with it's dependencies by calling
```
npm install
```
inside the project directory.

## Building and Watching

All `.scss` files stored in `css-source` that don't have a preceeding underscore, will be compiled to `.css` into the `css-output` directory. Anything with a preceeding underscore will be ignored, and is meant to only be imported by other `.scss` files. 

SASS files support importing both `.scss` and `.css` as SASS is backwards compatible with regular CSS.

You can build a css file from a the source directory by calling:
```
npm run build:sass
```

You can watch your source and build your source as you develop using:
```
npm run watch:sass
```

## Changing Input and Output directories
Configuration for the `build:sass` and `watch:sass` scripts are found inside the `package.json` file, under the `scripts` hash.
