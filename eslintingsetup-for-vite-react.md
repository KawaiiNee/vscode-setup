# vite - react eslinting setup

**install eslint**

```console
npm install --save-dev eslint-config-react-app eslint@^8.0.0
```

**create a .eslintrc.json file**

```jsx
// .eslintrc.json contents
{"extends": ["react-app", "react-app/jest"]}
```

**install a eslint plugin for vite using the following command**

```console
npm install --save-dev vite-plugin-eslint
```

**Once installed, add this to vite.config.js as plugin like so**

```jsx
import eslint from "vite-plugin-eslint";
// https://vitejs.dev/config/
export default defineConfig({
  plugins: [react(), eslint()],
});
```

### Refer
- https://stackoverflow.com/questions/69842785/how-can-i-intregate-eslint-in-a-vitereact-project
- https://www.npmjs.com/package/eslint-config-react-app
- https://www.npmjs.com/package/vite-plugin-eslint
