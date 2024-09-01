# Template for Rush Stack

## 简介

一个使用 [`Rush Stack`] 进行编排的 `Monorepos` 仓库。

作为模版创建当前仓库后，请修改修改 `rush.json` 中 `repository.url` 属性为实际仓库地址。(`SSH` 格式)

[`Rush Stack`](https://rushstack.io/)

## 操作说明详解

- 安装依赖

``` sh
rush update

# 清除缓存，重新安装
rush update -p

# 安装 rush-commitlint 的依赖
rush update-autoinstaller --name rush-commitlint
```

- 格式化当前代码

``` sh
rush prettier
```

- 发布仓库

``` sh
rush publish --apply --publish --add-commit-details --ignore-git-hooks --target-branch master
```
