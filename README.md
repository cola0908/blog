# Blog 我的博客

我的个人博客代码库，使用 [Hugo](https://github.com/gohugoio/hugo) 与 [Stack 主题](https://github.com/CaiJimmy/hugo-theme-stack) 构建。

部署在 Alibaba Cloud ESA（阿里云边缘安全加）上。

## 文章、页面编写流程

进入 Hugo 项目根目录：

```bash
cd /Users/cola_0908/Desktop/Develop/Blog
```

### 创建文章

文章目录使用英文短名称：

```bash
hugo new content post/my-first-post/index.md
```

初始默认文章模版生成位置：

```
content/post/my-first-post/index.md
```

编辑完成后，把文章开头：

```toml
draft = true
```

改为：

```toml
draft = false
```

## 创建文章

例如创建友链界面：

```bash
hugo new content page/friends/index.md
```

生成位置：

```
content/page/friends/index.md
```

## 本地预览

包含草稿：

```bash
hugo server -D --disableFastRender
```

浏览器打开：

```
http://localhost:1313/
```

不显示草稿：

```bash
hugo server --disableFastRender
```

## 正式构建

```bash
hugo --minify --cleanDestinationDir
```

生成的网站源码位于：

```
public/
```

## 提交至 Github

在 VS Code 中提交即可