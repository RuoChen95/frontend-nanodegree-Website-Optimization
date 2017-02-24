# frontend-nanodegree-Website-Optimization
##update:经过第一次审阅后我是如何修改的
###piza页面
- 在第486行将dom的操作放在循环之外
- 在第521行将layout的相关计算放在循环之外以防止重复计算
- 要求内容：将i的最大值调到24以下
- 在第551行删除var，防止多次声明
###个人介绍页面
- 第80行，将js文件本地化，具体文件从这里[https://github.com/eladkarako/reversed-engineered-google-analytics-js/blob/master/analytics.js]下
##如何打开文件:
- 将views/pizza.html用浏览器打开；
- 将index.html用浏览器打开

##我是如何优化index.html的
 - 去除外联css，减少搜索文件的时间
 - 将所有的js代码加上assync属性
 - 图片本地化
 
##我是如何优化views/js/main.js的:
- 将css文件以及js文件放到html的末尾；
- 修正changePizzaSizes，以解决dom的重复性选择以及FSL问题；
- 修正updatePositions：将layout的提取放在循环前面
