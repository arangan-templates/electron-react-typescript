# electron-react-typescript

An Electron app with react and TypeScript.

## Steps to do this from scratch

* `npx create-react-app my-app --use-npm --template typescript`
* cd my-app
* `npm install --save-dev electron`

## Additional files required by this project

* `tsconfig.json`
* `electron/tsconf.json`

## A few modifications to the package.json file

```json
scripts": {
    "start": "react-scripts start",
    "build:web": "PUBLIC_URL=./ react-scripts build",
    "build:desktop": "tsc -p electron/tsconf.json",
    "start:desktop": "npm run build:desktop && electron ./build/electron.js",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
  },
```

## Steps to do

* `npm run build:web`
* `npm run start:Desktop`
