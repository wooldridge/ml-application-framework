# ml-application-framework

## Clone project and install dependencies

```
git clone https://github.com/wooldridge/ml-application-framework
cd ml-application-framework
npm install
```

## Build the library

```
npm run build
```

This bundles the code in `/src` into a single `dist/bundle.js` library file.

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
