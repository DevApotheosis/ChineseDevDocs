# 文档构建的好手

> **程序员或许都不喜欢用HTML这种东西自己写文档吧，`mkdocs`这个Python模块，真的是一个天大的救星，这也是本网站构建所用的第三方库，真的相当好用**<br>

> **相关网站：[`mkdocs`官方Github仓库](https://github.com/mkdocs/mkdocs)**

## Mkdocs简介

**`MkDocs` 是一个基于 `Python` 的静态站点生成器，专门用于构建项目文档。它将 `Markdown` 格式的源文件转换为美观的静态 `HTML` 网站，并以一个简洁的 `YAML` 文件完成全部配置**<br>

**`MkDocs` 尤其受 `Python` 开发者喜爱，因为它的工作流程极其简单，且拥有强大的主题和插件生态。无论你是为开源项目编写技术手册、搭建团队内部知识库，还是创建个人博客，`MkDocs` 都是一个绝佳的选择**

## 核心特性/优点

1. **即时预览：`MkDocs` 内置了开发服务器，支持实时预览。当你保存文档更改时，浏览器会自动刷新，让你能即时看到效果**
2. **随处托管：`MkDocs` 生成的是完全静态的 `HTML` 站点，可以托管在 `GitHub Pages`、`Amazon S3` 或任何支持静态文件的服务器上**
3. **丰富的主题选择：`MkDocs` 内置了多款主题，包括默认的 `mkdocs` 主题和 `readthedocs` 主题。此外还有大量第三方主题可供选择，其中最受欢迎的是 `Material for MkDocs`，提供了现代化的 `Material Design` 风格**
4. **高度可定制：你可以通过自定义主题和安装插件来让文档呈现出你想要的样子。`MkDocs` 的插件生态非常丰富，涵盖站点管理、国际化、导航构建、`SEO` 优化等方方面面。**
5. **一键部署到 `GitHub Pages`：`MkDocs` 提供了 `gh-deploy` 命令，可以一键将站点部署到 `GitHub Pages`(白嫖党狂喜)**

## 安装与基础用法

**安装 MkDocs——首先确保系统已安装 Python 和 pip。然后使用 pip 安装：**

```bash
pip install mkdocs
```

**安装完成后，运行 mkdocs --version 验证是否安装成功，如果出现版本号，则说明安装成功**


