## 开发环境搭建

```bash
# 克隆项目
git clone ssh://git@gitlab.oopsdrone.top:47022/cmii-cloud/uav-web/cloud-platform.git

# 进入项目目录
cd cloud-platform

# 安装依赖
npm install

# 建议不要直接使用 cnpm 安装以来，会有各种诡异的 bug。可以通过如下操作解决 npm 下载速度慢的问题
npm install --registry=https://registry.npm.taobao.org

# 启动服务
npm run dev
```

浏览器访问 [http://localhost:9528](http://localhost:9528)

## 发布

```bash
# 构建测试环境
npm run build:stage

# 构建生产环境
npm run build:prod
```

## 其它

```bash
# 预览发布环境效果
npm run preview

# 预览发布环境效果 + 静态资源分析
npm run preview -- --report

# 代码格式检查
npm run lint

# 代码格式检查并自动修复
npm run lint -- --fix
```

> 关于使用git工具未校验问题参考 https://github.com/typicode/husky/issues/639 解决

## ICON使用

> 平台icon管理地址 https://www.iconfont.cn/manage/index?spm=a313x.7781069.1998910419.12&manage_type=myprojects&projectId=1642851

如有新增图标
1. 给icon命名(平台唯一)
2. 下载到本地替换 @asset/fonts 下文件

使用方式
```
# 单色icon
<i class="iconfont cmii-location"></i>

# 多色icon
<svg class="iconfont" aria-hidden="true">
    <use xlink:href="#cmii-location" />
</svg>
```

## 模块开发者

| 模块 | 前端开发者 | 接口服务开发者 |
| --------- | --------- | --------- |
| 空域服务 | 罗婷婷（luotingting） |  |
| 航线管理 | 陈龙（chenlong）刘芸志（liuyunzhi） |  |
| 作业管理 | 陈龙（chenlong）刘芸志（liuyunzhi） |  |
| 设备管理 | 李佩泽（ lipeizhe ）|  |
| 飞行监视 | 王清（wangqing）段峥祺（duanzhenqi） |  |
| 用户服务 | 王雄飞（wangxiongfei） |  |
| 飞手管理 |  |  |
| 个人系统 |  |  |
| 通知系统 |  |  |
| 告警系统 |  |  |
| 气象系统 |  |  |
| 审核系统 |  |  |


## Browsers support

Modern browsers and Internet Explorer 10+.

| IE / Edge | Firefox | Chrome | Safari |
| --------- | --------- | --------- | --------- |
| IE10, IE11, Edge| last 2 versions| last 2 versions| last 2 versions

# 测试地址
V1.1版本

 - 开发环境地址: http://192.168.11.191:8085/#/login
 - 测试环境地址: http://192.168.13.45:8185/#/login
 - 演示环境地址: 

V2.0版本

 - 开发环境地址: http://uavcloud.cmlc.dev.cc/
 - 测试环境地址: http://uavcloud.cmlc.test.cc/
 - 演示环境地址: http://cmlc.uav.cdcyy.cn:18000/#/login

## 分支说明

```bash
# 开发版本
git checkout develop

# 测试版本
git checkout staging

# 发布版本
git checkout master
```
# jingqu
