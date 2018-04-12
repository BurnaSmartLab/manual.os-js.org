# CLI

OS.js comes with a Node CLI utility that provides commands to manage your installation.

## Commands

All commands are provided via `npm` scipts:

* `build:manifest` - Builds package manifest (exposed to the client)
* `build:dist` - Builds core and all packages
* `watch:dist` - Same as build, but watches for changes
* `serve` - Starts the server
* `install:package` - Installs a package

## Examples

```
# Build everything
npm run build:dist

# Builds only core
npm run build:dist -- --core

# Builds given application
npm run build:dist -- --application=MyApplication

# Builds a set of application applications
npm run build:dist -- --applications=*
npm run build:dist -- --applications=MyApplication,MyOtherApplication

# Builds only applications
npm run build:dist -- --applications

# Builds only themes
npm run build:dist -- --themes

# Install a package
npm run install:package -- https://site/repo.git
```