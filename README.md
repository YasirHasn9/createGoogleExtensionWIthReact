# createGoogleExtensionWIthReact

Learn how to build a google extension With React and typescript

1. run `yarn create react-app 'name' --template typescript`
2. all you need now is to install `yarn add @types/chrome`
3. to make the extension works we need to optimize the `manifest.json` file in the `public` folder
4. In the `index.html` in the public folder, during the build time, react create-app embeds some script to
   reduce the HTTP requests, this leads to have some errors in the console. To unable that, optimize the `build` property in the
   `package.json` file and put at the beginning of the script a flag `INLINE_RUNTIME_CHUNK=false`
