# Docker Image - DocFx

DocFx is a Document generator for .Net Core a .Net Framework project

- For Use documentation refer to [DocFx Official Site](https://dotnet.github.io/docfx/).

## Instructions

You can build your document code with the following command:

```sh
docker run --rm --name docfx \
-v path-to-docs-folder:/docfx \
-v path-to-src-if-apply:container-src-path \
-w /docfx dynamicdevs/docfx:latest
```

### **Important**

- You should map document directory into `/docfx` directory.
- Whether your `src` folder is into directory `/docfx` folder don't map the `src` volume
- You should consider `-w` argument for executing docfx where docfx.json is located

## Plugins

- Plugins `memberpage`, `rest.operationpage`, `rest.tagpage` are in this image on the `/docfx/plugins` directory
