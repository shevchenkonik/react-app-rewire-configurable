# react-app-rewire-configurable

This package makes a part of modifications to react-scripts 2.0 to build custom configure

## Usage

**1. Install required dependencies**

```shell
npm i --save-dev react-app-rewired react-app-rewire-configurable
```

**2. Edit your `package.json` scripts to use `react-app-rewired` instead of `react-scripts`. [More information](https://github.com/timarney/react-app-rewired#3-flip-the-existing-calls-to-react-scripts-in-npm-scripts-for-start-build-and-test)**

```diff
  /* package.json */

  "scripts": {
-   "start": "react-scripts start",
+   "start": "react-app-rewired start",
-   "build": "react-scripts build",
+   "build": "react-app-rewired build",
-   "test": "react-scripts test --env=jsdom",
+   "test": "react-app-rewired test --env=jsdom",
    "eject": "react-scripts eject"
}
```

**3. You could add the following to your `package.json`**

```javascript
"config-overrides-path": "node_modules/react-app-rewire-micro-frontends",
```
