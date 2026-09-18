# 杨颖湄｜AI 测试工程师个人网站

这是一个纯 HTML / CSS / JavaScript 的本地简历网站，不需要安装前端依赖，也不需要 GitHub 才能查看。

## 本地查看

在项目根目录打开终端后运行：

```powershell
python -m http.server 5173
```

然后访问：

```text
http://localhost:5173/resume-site/
```

如果本机没有 Python，也可以使用任意静态文件服务器打开 `resume-site` 文件夹。

## 页面结构

- `index.html`：首页，只展示姓名、求职方向和核心能力
- `about.html`：关于我
- `experience.html`：工作与实习经历
- `projects.html`：项目列表，项目卡片可点击
- `project.html?id=lab`：项目详情模板，通过 URL 参数切换项目
- `skills.html`：测试能力
- `project-data.js`：项目背景、职责和测试关注点数据
- `styles.css`：整体视觉样式与移动端适配

项目详情示例：

```text
http://localhost:5173/resume-site/project.html?id=lab
```

目前项目详情页只使用脱敏文字，不放现公司内部截图或业务数据。

## 后续可补充

- 进一步确认并量化测试场景数量、缺陷发现数量和自动化效率
- 根据不同岗位制作手工测试版、AI 测试版两套内容
- 增加可脱敏的测试用例片段、接口测试示例或测试思路
- 增加 PDF 简历下载和可选的个人头像
- 后续如需公开部署，再配置 GitHub 或其他静态网站托管平台
