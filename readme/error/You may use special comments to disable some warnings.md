# You may use special comments to disable some warnings.
    0
        参考资料
            url
                https://www.jianshu.com/p/50e8818e3a85
    1
        在my-project项目添加了Hello.vue
            my-project/src/components/Hello.vue
                <template>
                    <div class="hello">
                        <h1>{{msg}}</h1>
                    </div>
                </template>
                
                <script>
                    export default {
                        name: "Hello",
                        data(){
                          return{
                            msg:'欢迎来到菜鸟教程！'
                          }
                        }
                    }
                </script>
                
                <style scoped>
                
                </style>

            my-project/src/router/index.js
                {
                  path: '/hello',
                  name: 'Hello',
                  component: Hello
                }
        启动就开始报错了
    2
        解决办法
            vue-cli脚手架关闭eslint的步骤：
            1
                打开 build文件夹下面的webpack.base.conf.js
                    my-project/build/webpack.base.conf.js
            2
                找到createLintingRule把代码注释掉
                        const createLintingRule = () => ({
                          /*test: /\.(js|vue)$/,
                          loader: 'eslint-loader',
                          enforce: 'pre',
                          include: [resolve('src'), resolve('test')],
                          options: {
                            formatter: require('eslint-friendly-formatter'),
                            emitWarning: !config.dev.showEslintErrorsInOverlay
                          }*/
                        })
    3
        重启项目
            正常。解决完毕