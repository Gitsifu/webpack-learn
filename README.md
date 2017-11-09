# webpack-learn

webpack学习

基于这篇[博客](https://segmentfault.com/a/1190000006178770)

[英文原文](http://www.pro-react.com/materials/appendixA/)

# windows跳坑

（由于此文章是基于Mac的）

文章最后执行`npm run build`是报错：

NODE_ENV不是内部或外部命令,也不是可运行的程序

解决办法：

安装across-env:`npm install cross-env --save-dev `

在运行命令加前缀：在`NODE_ENV=xxxxxxx`前面添加`cross-env`就可以了。 

例如：`"build": "cross-env NODE_ENV=production webpack --config ./webpack.production.config.js --progress"`

[解决方法原文](http://blog.csdn.net/koufulong/article/details/75270337)
