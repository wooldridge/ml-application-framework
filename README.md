# ml-application-framework

## Clone project and install dependencies

```
git clone https://github.com/wooldridge/ml-application-framework
cd ml-application-framework
npm install
```

## Build the library

**Option 1, using webpack:**

```
npm run build
```

This converts and bundles the code in `/src` into a single `/dist/index.js` library file. Set `ml-application-framework/package.json` to point to this:

```
"main": "dist/index.js",
```

**Option 2, using babel only:**

```
npm run babel
```

This converts and copies the code in `/src` into `/dist2`. Set `ml-application-framework/package.json` to point to this:

```
"main": "dist2/index.js",
```

## Set up example application

```
cd examples/ml-demo-app
npm install
```

Installed as a dependency is the library from above. See in `ml-demo-app/package.json`:

```
...
"ml-application-framework": "file:../..",
...
```

The `Test` component is imported and used in `App.js`.

## Run example application

```
npm start
```

Open application here: http://localhost:3000
