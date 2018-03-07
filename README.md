## 5se7en.com

nuxtjs+express+vue2.0+vuex搭建的服务端渲染个人网站项目.<br>
项目地址：https://5se7en.com/

## 注意事项

- node>=v8.0.0+ (nuxt1.0.0以上版本的node版本号必须大于v8.0.0否则启动的时候会报错)<br>
- 若要测试套马游戏登录请点击前往[套马游戏](https://www.hybjf.com/game/20170925Activity)注册一个账号

## 开发环境

- Node.js: `^8.9.4`
- express: `^4.16.2`
- nuxtjs: `^1.0.0-rc11`
- vue: `^2.5.3`

```bash
npm install
npm run dev
```

使用浏览器打开 `http://localhost:5757`

## 友情提示

- [N-blog](https://github.com/nswbmw/N-blog)(一个不错的Nodejs + Express + MongoDB入门项目)
- [vue2.0官网文档](https://vuejs.org/)
- [nuxtjs官方文档](https://nuxtjs.org/)
- [vue2-elm](https://github.com/bailicangdu/vue2-elm)(一个不错的vue2.0个人项目)
- [nuxtjs.org](https://github.com/nuxt/nuxtjs.org)

## nuxt介绍

- nuxt详细的入门教程这里不做详细的介绍，[官方文档](https://nuxtjs.org/)讲解的已经非常详细了。这里简单介绍一下项目目录作用

### nuxt目录介绍

- assets
    - 如果你的静态资源文件需要 Webpack 做构建编译处理，可以放到 assets 目录，否则可以放到 static 目录中去。
    - Nuxt 服务器启动的时候，该目录下的文件会映射至应用的根路径 / 下，像 robots.txt 或 sitemap.xml 这种类型的文件就很适合放到 static 目录中。

- components
    - 组件目录 components 用于组织应用的 Vue.js 组件。Nuxt.js 不会扩展增强该目录下 Vue.js 组件，即这些组件不会像页面组件那样有 [asyncData](https://nuxtjs.org/api/) 方法的特性。
    简而言之此目录就是普通的vue组件目录。

- layouts
    - 该目录名为Nuxt.js保留的，不可更改。
    - 你可以自定义合适自己网站的默认样式和错误样式

- middleware
    - 中间件执行流程顺序：
        - nuxt.config.js
        - 匹配布局
        - 匹配页面

- pages
    - 该目录名为Nuxt.js保留的，不可更改。
    - 页面目录 pages 用于组织应用的路由及视图。Nuxt.js 框架读取该目录下所有的 .vue 文件并自动生成对应的路由配置。
    - 此页面的.vue文件都具有[asyncData](https://nuxtjs.org/api/)、[fech](https://nuxtjs.org/api/pages-fetch)方法。

- plugins
    - 插件目录 plugins 用于组织那些需要在 根vue.js应用 实例化之前需要运行的 Javascript 插件。
    - 我们可以将element-ui或者mint-ui以及其他更多的插件都可以放在plugins中使用

- static
    - 该目录名为Nuxt.js保留的，不可更改。
    - 静态文件目录 static 用于存放应用的静态文件，此类文件不会被 Nuxt.js 调用 Webpack 进行构建编译处理。 服务器启动的时候，该目录下的文件会映射至应用的根路径 / 下。

- store
    - 该目录名为Nuxt.js保留的，不可更改。
    - store 目录用于组织应用的 Vuex 状态树 文件。 Nuxt.js 框架集成了 Vuex 状态树 的相关功能配置，在 store 目录下创建一个 index.js 文件可激活这些配置。

### nuxt配置介绍





