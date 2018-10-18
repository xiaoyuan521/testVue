# testVue


1：安装vue的环境参照地址 https://segmentfault.com/a/1190000014211773

    先去官网下的node js 并安装 参照地址 https://segmentfault.com/a/1190000013950461

    输入以下命令npm -g install npm，更新npm至最新版本。
    不用安装淘宝镜像  用正常的npm安装即可
    安装vue 脚手架 输入命令 npm install -g vue-cli 
    
    新建项目的时候 用命令 vue init webpack demo(你新建的项目名称/文件名称)
    
    继续执行： cd demo (这是进入到demo文件夹的命令)

     然后执行 安装 ：npm install
     
     npm run dev 运行项目
      http://localhost:8080 查看效果
      
      
      如果需要 ajax 安装  npm install axios
      main.js  文件里面 axios.defaults.baseURL = 'https://localhost:8443/api' 尽量不要加https 用 http
      
2：搭建后台spring boot 参照地址
       https://www.cnblogs.com/ityouknow/p/5662753.html
       和https://blog.csdn.net/liutong123987/article/details/79385513
      
3：前台 用npm run dev 启动 然后调前台代码

4：后来用spring boot启动 调后端代码 注意 这俩端口号要区分 还需要支持跨域

5：如果前台调试好了 进入工程目录    npm run build命令进行打包，会自动生成打包后的dist目录文件。

  然后把dist里面所有文件都拷贝到springboot项目的resources/static目录下

6：然后重启springboot项目，浏览器访问后台服务地址：https://localhost:8443
  会发现页面显示的就是vue开发的前端页面，然后输入用户名密码登录正常。
  
  注意 浏览器上面的#是固定的 写法 也可以去掉 在router下面的 index.js 里面加 mode="history";(有一个问题就是后台启动项目的时候 刷新页面会报404，具体处理方法还没研究)
  
  
