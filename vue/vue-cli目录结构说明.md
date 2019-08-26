@vue/cli笔记
=====
## 目录结构  
 - public:静态资源目录，不会被Webpack打包
 - src:入口文件和组件文件
   - assets:图片和静态资源等
   - components:自定义功能组件
   - views:公共组件
 - App.vue:根组件，也是所有组件的出口,会被渲染到index.html的dom结构中
 - main.js:入口文件,在这里去引入App组件,路由组件,需要全局使用的东西都可以定义在这里
 - router.js:路由文件,路由配置在这
 - store.js:Vuex文件  
 - package.json:npm创建的文件,里面定义了项目名、版本以及相关依赖等等
   - dependencies:依赖项
   - devDependencies:开发环境所需的依赖
 - package-lock.json:npm创建,用来锁定安装的包的版本