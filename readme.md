# Tobub Douyin Skills

抖音（Douyin）浏览器自动化与数据采集 Skill 集合，基于 Tobub Skill Package 规范构建。

这些 Skill 以可导入的 `.skill.json` 文件提供，用于自动化浏览抖音视频、获取视频下载地址、读取评论、搜索结果、用户作品和用户信息。

注意：skill使用基于免费工具tobub （可以api和桌面应用使用）

https://github.com/pow505/tobub

## Features

- 抖音视频自动化浏览
- 获取抖音视频播放和下载地址
- 获取视频作品评论
- 获取抖音搜索结果
- 获取用户发布的作品
- 获取抖音用户信息
- 采集结果保存到 Tobub 数据库
- JSON Skill Package，可直接导入 Tobub
- 支持浏览器自动化和网络响应捕获
- `downloadUrls` 保留原始数组，同时提供 `download1`、`download2`、`download3` 方便复制和访问

## Included Skills

| Skill | Description | Main Output |
| --- | --- | --- |
| 抖音自动化浏览视频 | 自动浏览抖音视频列表并采集作品信息 | `records` |
| 抖音获取下载地址 | 获取指定视频的播放和下载地址 | `downloadUrls`, `download1`, `download2`, `download3` |
| 抖音获取作品评论 | 获取指定视频的评论数据 | `videoId`, `records` |
| 抖音获取搜索结果 | 根据关键词搜索抖音内容 | `query`, `records`, `scans` |
| 抖音获取用户作品 | 获取指定用户发布的视频作品 | `user`, `records` |
| 抖音获取用户信息 | 获取指定用户的公开资料 | `user` |

## Repository Structure

```text
tests/抖音/
├── 抖音自动化浏览视频.skill.json
├── 抖音获取下载地址.skill.json
├── 抖音获取作品评论.skill.json
├── 抖音获取搜索结果.skill.json
├── 抖音获取用户作品.skill.json
└── 抖音获取用户信息.skill.json
