<div align="center">
<h1>Type definitions for XML DOM</h1>
</div>

![](https://img.shields.io/github/package-json/v/Ziphil/ZenmlXmldomType)
![](https://img.shields.io/github/commit-activity/y/Ziphil/ZenmlXmldomType?label=commits)


## Overview
The type definition file for `@xmldom/xmldom` loads the built-in type definitions (namely `lib.dom.d.ts`).
These type definitions are, however, meant to be used for scripts that will run in a browser, so they are not appropriate when using `@xmldom/xmldom` on Node.js.
For example, the built-in typedefs have the `Element.insertAdjacentElement` method, but `@xmldom/xmldom` does not provide it.

This package provides the appropriate type definitions for `@xmldom/xmldom` on Node.js.
Use it to replace the built-in `lib.dom.d.ts`.

This is also a part of the [ZenML](https://github.com/Ziphil/Zenml) infrastructure.

## Installation and usage
Make sure that the version of your TypeScript is 4.5 or above.
Add the following code to your `package.json` and run `npm install`.
```json
"dependencies": {
  "@typescript/lib-dom": "npm:@zenml/xmldom-type",
}
```

For further information on type definition overriding, see [this announcement](https://devblogs.microsoft.com/typescript/announcing-typescript-4-5-beta/#supporting-lib-from-node_modules) or [the pull-request page for this feature](https://github.com/microsoft/TypeScript/pull/45771).