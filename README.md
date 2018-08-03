# @ucudal/eslint-config

This package provides UCUDAL's base JavaScript `.eslintrc` as an extensible
shared config.

## Usage

1. Install the correct versions of each peer dependency, which are listed by the
   command:

```sh
npm info "@ucudal/eslint-config@latest" peerDependencies
```

Linux/OSX users can run:

```sh
(
  export PKG=@ucudal/eslint-config;
  npm info "$PKG@latest" peerDependencies --json | command sed 's/[\{\},]//g ; s/: /@/g' | xargs npm install --save-dev "$PKG@latest"
)
```

Which produces and runs a command like:

```sh
  npm install --save-dev @ucudal/eslint-config@latest eslint@^#.#.#
```

Windows users can install the `@ucudal/eslint-config` and all its peer
dependencies manually.

2. Add `"extends": "@ucudal"` to your `.eslintrc` file.
