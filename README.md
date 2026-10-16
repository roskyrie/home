# 沈伟 · Shen Wei

个人科研主页，展示机器人导航、异构机器人、多智能体协同与仿真学习相关经历。

**主页：** [https://roskyrie.github.io/home/](https://roskyrie.github.io/home/)

## 页面内容

- 关于我与研究方向
- ROS 2 自动巡检智能车、校园巡检无人系统、机器人仿真与学习
- 实验影像：47 张导航感知、协同调度与机器人仿真图片，支持筛选和点击放大
- 北京航空航天大学、杭州电子科技大学教育经历
- 编程与机器人开发工具、英语成绩及奖学金
- 邮箱、电话／微信及 GitHub 联系方式

页面文字和图片根据本人提供的简历整理。进行中的学习和实验按探索性工作表述；未添加论文、性能指标或未经提供的经历。原始简历 PDF 未上传至仓库。补充展示图片来自本人指定的 workasset 目录；源码、模型、训练日志和录屏未公开上传。

## 本地预览

无需安装前端依赖或构建，直接启动静态文件服务器：

```bash
python3 -m http.server 3000
```

打开 `http://localhost:3000/`。

## 文件结构

```text
index.html                    页面内容与轻量导航脚本
static/css/profile.css        科研主页样式与移动端适配
static/img/           个人照片与简历中的项目图片
static/img/avatar.svg         网站图标
.github/workflows/deploy.yml  GitHub Pages 自动部署
```

`static/css/index.css` 保留原始模板样式，当前页面使用 `profile.css`。

## 修改与发布

直接修改 `index.html` 中对应的文字、链接和图片。更新 `static/css/profile.css` 可调整布局和配色。

GitHub 仓库为 `roskyrie/home`，Pages 发布源为 **GitHub Actions**。推送到 `master` 或 `main` 后，工作流自动部署到主页地址。

原巡检项目源码链接按简历保留为 `Kobe24forever263/Learn_ros_patrol`；该项目属于另一个 GitHub 账号，不能仅因主页迁移而替换其所有者。

## 致谢与许可

本项目基于 [quietseek/home](https://github.com/quietseek/home) 模板改造。保留原始 [MIT License](LICENSE) 及其版权声明。个人照片与项目图片来自本人提供的简历，MIT 许可不构成对肖像或第三方素材权利的额外授权。
