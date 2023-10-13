# `attw` issue

This repository is created to reproduce an import issue with `attw`. It is a TypeScript monorepo that uses Yarn workspaces.

## Install
```bash
yarn install
```

## Issue Description

The issue occurs when attempting to resolve imports in the code scanned by `attw`. Specifically, it seems to happen only with "long" paths. The repository contains four packages, each testing a different use case. These use cases involve different folder and file name lengths.

## Usage

To test each use case, you can run the following command:

```bash
yarn workspace [package] attw
```

## Packages

1. `works`: A package where imports work correctly.
2. `works-2`: Another package with working imports.
3. `fails`: A package that demonstrates the import issue.
4. `fails-2`: Another package that reproduces the import issue.

Feel free to explore and test each package to replicate and understand the issue with `attw`.
