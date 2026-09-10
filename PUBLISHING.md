# Building and Publishing

Requires Node.js, npm, and [Task](https://taskfile.dev/). Install the dependencies with:

```sh
npm ci
```

Generate the language data and build the VSIX package:

```sh
task generate
task build
```

To publish to the Visual Studio Marketplace and Open VSX, set `VSCE_PAT` and `OVSX_PAT`, then run:

```sh
task publish
```

To publish to a single marketplace:

```sh
task publish:marketplace
task publish:openvsx
```
