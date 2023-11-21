Steps to reproduce the error:
Execute the following commands:
```
nvm use

npm ci

npm run build
```

It should show several errors like to following one:
```
"/*@__PURE__*/"

in "node_modules/@stencil/core/internal/client/index.js" contains an annotation that Rollup cannot interpret due to the position of the comment. The comment will be removed to avoid issues.
```

[Here](https://github.com/intlify/vue-i18n-next/issues/1599) you can find a detailed explanation of why the error occurs and how to fix it.
