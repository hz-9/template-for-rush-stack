# Template for Rush Stack

## Introduction

A `Monorepos` repository orchestrated using [`Rush Stack`].

After creating the repository from this template, please modify the `repository.url` property in `rush.json` to the actual repository address. (`SSH` format)

[`Rush Stack`](https://rushstack.io/)

## Detailed Instructions

- Install dependencies

``` sh
rush update

# Clear cache and reinstall
rush update -p

# Install dependencies for rush-commitlint
rush update-autoinstaller --name rush-commitlint
```

- Format the current code

``` sh
rush prettier
```

- Publish the repository

``` sh
rush publish --apply --publish --add-commit-details --ignore-git-hooks --target-branch master
```
