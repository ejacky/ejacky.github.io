---
title: "用 hugo 在 Github Pages 上发布博客"
date: 2022-03-17T14:00:45+08:00
draft: true
---
# 
- hugo 安装成功

````
hugo new post/xx.md // 创建文章
hugo server -D // 本地启动服务调试
hugo -D        // 生成静态文件到 public/ 目录
````

# 问题
- deploy 一致失败，报以下错误
```
Creating deployment with payload:
{
	"artifact_url": "https://pipelines.actions.githubusercontent.com/i7NDiJe6sckpMiQgKJEPbHK39ol64joVbrfBfWuElGyIPZzm9e/_apis/pipelines/1/runs/13/artifacts?artifactName=github-pages&%24expand=SignedContent",
	"pages_build_version": "26b486ee6204e9df792692b5a91daffc45880070",
	"oidc_token": "***"
}
Failed to create deployment for 26b486ee6204e9df792692b5a91daffc45880070.
{"message":"Deployment request failed for 26b486ee6204e9df792692b5a91daffc45880070 due to in progress deployment. Please cancel 8e52d20341103fba0f42d25d5c4e3a6a716b897b first or wait for it to complete.","documentation_url":"https://docs.github.com/rest/reference/repos#create-a-github-pages-deployment"}
Error: Error: Request failed with status code 400
Error: Error: Request failed with status code 400
Sending telemetry for run id 1997691410
```

- 日期显示问题
- about 导航没出现
- 首页每篇文章展示首段，可仿照 [月光博客](https://www.williamlong.info/ )


