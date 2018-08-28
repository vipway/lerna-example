## 初始化git项目
`git init lerna-example`

## `cd lerna-example` 初始化lerna

`lerna init`

## 进入 packges文件夹

`cd packges` 

## 初始化npm包 lerna-exp-a, lerna-exp-b 默认使用版本号：0.0.1

`cd lerna-exp-a`

`npm init`

`cd ../lerna-exp-b`

`npm init`

## `lerna-exp-a` 添加 pakcge.json 添加依赖

`dependencies:{"lerna-exp-b": "^0.0.1"}`

## 执行 

`lerna bootstrap`

## 关连远程git

`git add -A`

`git commit -m test`

`git remote add origin https://github.com/vipway/lerna-example.git` (此仓库应为实际测试仓库地址)

`git push --set-upstream origin master`

## 发布至npm，添加`--skip-git`则不提交至远程git

`lerna publish --skip-git`

## 进入 lerna-exp-b文件夹，编辑 index.js 插入代码 `console.log('update')` 保存，执行

`git add -A`

`git commit -m update`

## 返回根目录，提交代码至git并更新npm包。根据提示，输入更新版本号，完成更新

`lerna publish`




