# @esm2cjs/indent-string

This is a fork of https://github.com/sindresorhus/indent-string, but automatically patched to support ESM **and** CommonJS, unlike the original repository.

## Install

You can use an npm alias to install this package under the original name:

```
npm i indent-string@npm:@esm2cjs/indent-string
```

```jsonc
// package.json
"dependencies": {
    "indent-string": "npm:@esm2cjs/indent-string"
}
```

but `npm` might dedupe this incorrectly when other packages depend on the replaced package. If you can, prefer using the scoped package directly:

```
npm i @esm2cjs/indent-string
```

```jsonc
// package.json
"dependencies": {
    "@esm2cjs/indent-string": "^ver.si.on"
}
```

## Usage

```js
// Using ESM import syntax
import indentString from "@esm2cjs/indent-string";

// Using CommonJS require()
const indentString = require("@esm2cjs/indent-string").default;
```

> **Note:**
> Because the original module uses `export default`, you need to append `.default` to the `require()` call.

For more details, please see the original [repository](https://github.com/sindresorhus/indent-string).

## Sponsoring

To support my efforts in maintaining the ESM/CommonJS hybrid, please sponsor [here](https://github.com/sponsors/AlCalzone).

To support the original author of the module, please sponsor [here](https://github.com/sindresorhus/indent-string).
