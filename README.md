# qft-uniapp

## 1. 安装依赖 如果安装报错建议升级node版本：16.17.0  npm版本：8.15.0
npm install


## 2. 启动H5端
npm run dev:h5


## 3. 打包H5
npm run build:h5 


## 4. 运行APP
npm run dev:app
-使用USB连接手机和电脑，运行以上命令后会在项目目录中生成 dist\dev\app
-使用Hbuilderx 打开该目录-工具栏-'运行'-'运行到手机或模拟器'-'运行到Android App基座' / '运行到IOS App基座'


## 5. 打包APP
npm run build:app
-使用npm run build:app会在/dist/build/app下生成app打包资源。如需制作wgt(增量)包，将app-plus中的文件压缩成zip 可以使用Bandizip压缩工具
-（注意：不要包含app目录），再重命名为${appid}.wgt， appid为manifest.json文件中的appid。
-也可以使用HBuilder工具压缩-打开HBuilder -> 导入该项目 -> 选中该项目目录 -> 发行 -> 原生App-制作应用wgt包 ->确定

-注意：使用 HBuilder打包需要控制HBuilder的版本与APP的SDK版本保持一致，不然无法运行


## 6. 下拉刷新 上拉加载更多组件地址 https://z-paging.com/start/intro.html
-在线demo地址 https://demo.z-paging.zxlee.cn/#/  
-demo下载地址 https://ext.dcloud.net.cn/plugin?id=3935


## 7. 组件命名规范
-全局组件遵守uniapp命名规范 components目录下 comp-组件名称/comp-组件名称.vue
-只要组件路径符合规范，就可以不用引用、注册，直接在页面中使用。
-不管components目录下安装了多少组件，打包会自动剔除没有使用的组件，对组件库的使用尤为友好。


## 8. git 代码提交规范遵从以下规则：
-* feat：新增功能
-* fix：bug 修复
-* docs：文档更新
-* style：不影响程序逻辑的代码修改(修改空白字符，格式缩进，补全缺失的分号等，没有改变代码逻辑)
-* refactor：重构代码(既没有新增功能，也没有修复 bug)
-* perf：性能, 体验优化
-* test：新增测试用例或是更新现有测试
-* build：主要目的是修改项目构建系统(例如 glup，webpack，rollup 的配置等)的提交
-* ci：主要目的是修改项目继续集成流程(例如 Travis，Jenkins，GitLab CI，Circle等)的提交
-* chore：不属于以上类型的其他类型，比如构建流程, 依赖管理
-* revert：回滚某个更早之前的提交
-注意 冒号是英文冒号


## 9. 单位尺寸规范
-uniapp中统一使用rpx单位，目的是为了兼容不同型号的手机
-两者间属于近2倍关系- 10px约等于20rpx 

