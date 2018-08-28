## 初始化git项目
`git init <repository name>` 

## 初始化 lerna 
`lerna init`

## 进入 packges文件夹

`cd packges` 

## 初始化npm包(npm init命令) lerna-exp-a, lerna-exp-b   ps: 不懂度娘～～～

`cd lerna-exp-a`
`npm init`
`cd ../lerna-exp-b`
`npm init`

## `lerna-exp-a` 添加 pakcge.json 添加依赖

`dependencies:{"lerna-exp-b": "^0.0.1"}`

## 执行 

`lerna bootstrap`

## 关键远程git




