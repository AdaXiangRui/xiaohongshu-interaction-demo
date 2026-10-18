# 小红书交互 Demo

这是一个无需安装依赖即可运行的静态前端 Demo，包含：

- 发现首页
- 个人主页
- 消息页
- 市集页
- 视频详情页
- 图文笔记详情页
- 评论展开页
- 页面跳转、返回、点赞和收藏状态交互
- 参考录屏实现的爱心点赞动效：主心形回弹、粒子散开、数字加一
- 视频页支持点击底部爱心或双击画面点赞

项目的 AI / Coding 工具分工、需求迭代和制作过程见 [`AI-Coding制作过程.md`](AI-Coding制作过程.md)。

## 本地运行

最简单的方式是直接双击 `dist/index.html`。

如果浏览器限制本地资源，可在项目目录运行一个静态服务器：

```bash
python3 -m http.server 8000 --directory dist
```

然后打开：

```text
http://localhost:8000
```

## 文件结构

```text
AI-Coding制作过程.md  AI / Coding 工具与制作过程说明
dist/
  index.html       页面入口
  styles.css       全部视觉样式
  app.js           路由、页面模板和交互逻辑
  assets/          页面图片素材
.openai/
  hosting.json     Sites 部署配置
```

## 修改页面

- 页面内容及交互：编辑 `dist/app.js`
- 视觉样式：编辑 `dist/styles.css`
- 图片素材：替换 `dist/assets/` 中对应文件

已发布的私有 Demo：

https://xiaohongshu-interaction-demo.hazyoak.chatgpt.site
