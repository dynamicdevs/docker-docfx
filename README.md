# Docker Image - DocFx

DocFx is a Document generator for .Net Core a .Net Framework project

- For Use documentation refer to [DocFx Official Site](https://dotnet.github.io/docfx/).

## Instructions

You can build your document code with the following command:

```sh
docker run --rm --name docfx -v path-to-docs-folder:/docfx-js-ts -v path-to-src-if-apply:dest-in-src -w /docfx dynamicdevs/docfx-js-ts:latest docfx docfx.json build
```

### **Important**

You should map document directory into `/docfx` directory.

## Plugins

- Plugins `memberpage`, `rest.operationpage`, `rest.tagpage` are in this image on the `/docfx/plugins` directory