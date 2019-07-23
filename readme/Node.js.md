# Node.js
    0
        参考资料
            url
                https://www.runoob.com/nodejs/nodejs-tutorial.html
    1
        介绍
            Node.js 就是运行在服务端的 JavaScript。
            Node.js 是一个基于Chrome JavaScript 运行时建立的一个平台。
            Node.js是一个事件驱动I/O服务端JavaScript环境，基于Google的V8引擎，V8引擎执行Javascript的速度非常快，性能非常好。
    2
        下载
            https://nodejs.org/en/
    3
        安装
    4
        查看使用的版本
            # 查看版本
                Microsoft Windows [版本 10.0.17763.615]
                (c) 2018 Microsoft Corporation。保留所有权利。
                
                C:\Users\h_don>node -v
                v10.16.0
                
                C:\Users\h_don>npm -v
                6.9.0
                
                C:\Users\h_don>
        查看Node以及NPM版本
# NPM 使用介绍
    1
        NPM是随同NodeJS一起安装的包管理工具，能解决NodeJS代码部署上的很多问题，常见的使用场景有以下几种：
            允许用户从NPM服务器下载别人编写的第三方包到本地使用。
            允许用户从NPM服务器下载并安装别人编写的命令行程序到本地使用。
            允许用户将自己编写的包或命令行程序上传到NPM服务器供别人使用。
        由于新版的nodejs已经集成了npm，所以之前npm也一并安装好了。同样可以通过输入 "npm -v" 来测试是否成功安装。
            # 查看版本
                Microsoft Windows [版本 10.0.17763.615]
                (c) 2018 Microsoft Corporation。保留所有权利。
                
                C:\Users\h_don>npm -v
                6.9.0
                
                C:\Users\h_don>
    2
        2.1
            cnpm介绍
                淘宝定制的 cnpm (gzip 压缩支持) 命令行工具代替默认的 npm
            #升级或安装 cnpm
                npm install cnpm -g
                    C:\Users\h_don>npm install cnpm -g
                    C:\Users\h_don\AppData\Roaming\npm\cnpm -> C:\Users\h_don\AppData\Roaming\npm\node_modules\cnpm\bin\cnpm
                    + cnpm@6.1.0
                    added 691 packages from 924 contributors in 219.313s
                    
                    C:\Users\h_don>
        2.2
            #升级 npm
                cnpm install npm -g
            #升级之后查看npm版本由6.9.0变成了6.10.1
                C:\Users\h_don>npm -v
                6.10.1
    3
        在用 Vue.js 构建大型应用时推荐使用 NPM 安装：
            # 最新稳定版
            cnpm install vue