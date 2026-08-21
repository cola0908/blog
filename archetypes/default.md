+++
# 文章日期配置，自动生成创建时间
date = '{{ .Date }}'

# 新文章默认是草稿
draft = true

# 根据文件名生成标题
title = '{{ replace .File.ContentBaseName "-" " " | title }}'

# 文章摘要和 SEO 描述
description = ""

# URL 短链接，留空根据文件名生成
slug = ""

# 文章封面图，相对于文章目录
image = ""

# 文章分类
categories = []

# 文章标签
tags = []

# 是否显示目录
toc = true

# 是否自动渲染数学公式
math = false

# 是否启用评论，仍受全站评论开关控制
comments = true
+++
