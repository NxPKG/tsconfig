
# Nxpkg tsconfig

[![npm](https://img.shields.io/npm/v/@nx-pkg/tsconfig.svg)](https://www.npmjs.com/package/@nx-pkg/tsconfig)
[![downloads](https://img.shields.io/npm/dt/@nx-pkg/tsconfig.svg)](https://www.npmjs.com/package/@nx-pkg/tsconfig)
[![build](https://travis-ci.org/nxpkg/tsconfig.svg?branch=master)](https://travis-ci.org/nxpkg/tsconfig)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)

Base tsconfig.json for TypeScript projects at Nxpkg.
It only includes compiler options that make TypeScript more strict.
It does not set any project-specific or environmental settings.

## Usage

```
npm install --save-dev @nx-pkg/tsconfig
```

Then add this tsconfig.json:

```json
{
  "extends": "./node_modules/@nx-pkg/tsconfig/tsconfig.json"
}
```

## Making changes

```
npm link
cd <project>
npm link @nx-pkg/tsconfig
npm run lint
```

## Publish a new version

Follow [semver](http://semver.org/).

```
npm version major|minor|patch
git push
git push --tags
npm publish
```

