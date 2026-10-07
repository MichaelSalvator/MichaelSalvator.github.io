# 个人主页（Academic Pages）

这是用 [Academic Pages](https://github.com/academicpages/academicpages.github.io) 模板搭建的学术个人主页，内容已按你的简历填好：8 篇已发表/已接收论文、5 篇在投论文、7 次会议、CV 页面和左侧个人信息栏。

## 一、怎么上线（大约 5 分钟）

1. 注册并登录 [GitHub](https://github.com)（邮箱要验证）。
2. 右上角 **+ → New repository**，仓库名必须写成 `<你的用户名>.github.io`（例如用户名是 `wyaoru`，仓库名就是 `wyaoru.github.io`），设为 **Public**，不要勾选 Add a README。
3. 进入新建的空仓库，点 **Add file → Upload files**，把本文件夹里的**所有文件和文件夹**拖进去，Commit。
4. 进仓库 **Settings → Pages**，Source 选 **Deploy from a branch**，Branch 选 **main**、目录选 **/(root)**，Save。
5. 等 1–2 分钟，访问 `https://<你的用户名>.github.io` 就能看到主页了。

> 之后每次在网页上改文件并提交，网站会自动重新生成，不需要额外操作。

如果觉得网页上传太慢，也可以装一个 **GitHub Desktop**，用它把本文件夹添加成本地仓库再 Push，效果一样。

## 二、还需要你补的东西

| 要补什么 | 在哪里改 | 状态 |
| --- | --- | --- |
| 邮箱、ORCID | `_config.yml` 的 `author:` 部分 | 已填 |
| 侧边栏头像 | `images/profile.png` | 已用蓝底证件照替换 |
| 简历 PDF | `files/cv.pdf` | 已放入 |
| ResearchGate 主页 | `_config.yml` 的 `researchgate` | 已填 |
| Google Scholar | — | 按要求不使用（`googlescholar` 留空） |
| 手机号 | 简历 docx | 已统一为 15708998908 |

GitHub 用户名已经填好了（`MichaelSalvator`），所以仓库名要建成 `MichaelSalvator.github.io`，网站地址是 https://michaelsalvator.github.io 。

没有填的社交链接不会显示，也不会产生空按钮，所以可以先只填邮箱。

> 侧边栏头像目前是一张写着 "WY" 的占位图。你的 GitHub 头像是一张简单的图形，不太适合当作学术主页的正式照片，所以没有用它，建议换成你自己的证件照或生活照。

## 三、目录结构

```
_config.yml          站点总配置：名字、简介、侧边栏、社交链接
_data/navigation.yml 顶部导航（目前是 Publications / Talks / CV）
_pages/
  about.md           首页：个人简介、研究兴趣、动态、教育背景、代表论文
  cv.md              CV 页面（论文和会议会自动生成列表）
  publications.html  论文列表页
  talks.html         会议列表页
_publications/       每篇论文一个 Markdown 文件
_talks/              每次会议一个 Markdown 文件
images/profile.png   侧边栏头像（蓝底证件照裁成 400×400）
images/photo-casual.jpg  首页正文右侧浮动的生活照
files/cv.pdf         简历 PDF，CV 页面的下载按钮指向这里
```

首页和 CV 页里都有一个 **Code and data** 小节，链接到你 GitHub 上的 MFSET、HESPERIA 和 MRMS-GRU 三个仓库。

## 四、以后怎么加内容

**加一篇论文**：在 `_publications/` 里新建一个文件，例如 `2026-12-01-my-new-paper.md`，内容照抄下面这份再改字段：

```yaml
---
title: "论文标题"
collection: publications
category: manuscripts      # manuscripts=期刊论文, conferences=会议论文, under-review=在投
permalink: /publication/2026-my-new-paper
excerpt: '一句话摘要'
date: 2026-12-01
venue: '期刊名称'
paperurl: 'https://doi.org/...'
citation: '作者. (2026). &quot;论文标题.&quot; <i>期刊名称</i>. 卷(期), 页码.'
---
```

**加一次会议**：在 `_talks/` 里新建文件，字段参考已有的条目，`type` 可以写 `Oral presentation`、`Poster` 或 `Conference attendance`。

**改顶部导航**：编辑 `_data/navigation.yml`，删掉一行就能去掉一个菜单项。

## 五、本地预览（可选，不做也没关系）

上线不依赖本地环境。如果你想在自己电脑上先看效果，需要装 Ruby 和 Bundler，然后在终端里执行：

```bash
bundle install
bundle exec jekyll serve
```

然后打开 http://localhost:4000 。

## 六、说明

- 论文的 `paperurl` 已核对到真实的 DOI，可以直接点开。
- 会议只写到年份，因为原始材料里没有具体日期；有准确日期的话把 `date` 改成 `2025-08-15` 这种格式即可（页面上目前只显示年份）。
- 论文的 `date` 目前用的是年份对应的一月一日，用来排序，页面上也只显示年份。
