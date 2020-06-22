# fastroll

Rollup modules without configuration

## Install

```
$ npm i -g fastroll
```

## Use

```
$ fastroll lib.js --format es --output lib.es.js
$ fastroll lib.js --format cjs --exclude path --exclude os --output dist/lib.js
$ fastroll lib.js --format umd --name lib --output lib.umd.js
```

Fastroll makes it possible to create Rollup bundles with single one-line command, just like Browserify. To achieve this Fastroll ships with a number of Rollup plugins already installed and preconfigured:

- `@rollup/plugin-commonjs`
- `@rollup/plugin-json`
- `@rollup/plugin-node-resolve`
- `rollup-plugin-node-builtins`
- `rollup-plugin-node-globals`

The command exposes the following options to customize the behaviour of Rollup and these plugins:

```
--output, -o    Output bundle target file
--format, -f    Format to use for output bundle
--name, -n      Name of the bundle export
--exclude, -e   External module(s) to exclude from bundle
--mode, -m      Export mode to use for bundle
--help, -h      Display command help information
```

## License

Apache-2.0
