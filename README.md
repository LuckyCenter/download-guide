## 一个下载引导页
> 一个用于指导用户下载客户端软件及指导用户使用的一个网站，独立于主系统之外。这里主要用到node后台技术来实现功能。
### 技术：node + express + pm2 + jade + morgan
> - node:一个开源与跨平台的 JavaScript 运行时环境；
> - express:基于node平台的web应用开发框架；
> - pm2:带有负载均衡功能的node应用的进程管理器。pm2-windows-startup是它配套的windows自启动包；
> - jade:基于node环境的前端模板引擎，可根据特定的语法规则生成html文档；
> - morgan:express默认的日志中间件，用来记录日志，也可以脱离express，作为node.js的日志组件单独使用。

### 启动步骤
1. npm install
2. npm install pm2 -g
3. 进入 download-guide 根目录找到run.bat，双击运行。
4. 在浏览器地址栏输入 localhost （或者自己电脑的IP），即可看到引导页。说明运行成功。
5. 在cmd输入 pm2 ls 可查看当前运行在pm2上的进程，并通过pm2命令来管理进程。

### pm2常用命令
- pm2 ls 查看所有进程
- pm2 stop all 停止所有进程
- pm2 stop 0 停止指定进程
- pm2 delete 0 杀死指定进程
- pm2 restart 0 重启所有进程
