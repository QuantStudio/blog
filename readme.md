# QuantStudio Blog

## 开发环境搭建

> php 7.1+
> node 8+

- 拉取代码
- 展开项目
  - composer install
  - npm ci

## 发布流程

`npm run production`

`git add -f build_production && git commit -m "build for publish"`

`git subtree push --prefix build_production gh-pages master`

其中 gh-pages 为地址是 https://github.com/QuantStudio/quantstudio.github.io 的 git remote
