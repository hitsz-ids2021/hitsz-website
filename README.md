# 哈尔滨工业大学数据安全研究院


## 如何在本地初始化？

## 如何修改主页？

在这之前，我们先来熟悉一下整个文件目录。

```bash
├── config
├── content
│   ├── accomplishments
│   ├── authors
│   ├── home
|   ├── members
|   ├── publications
|   ├── talks
├── data
├── docs
├── resources
├── scripts
├── static
├── themes
├── .editorconfig
├── .gitignore
├── .gitmodules
├── generate.bat
├── LICENSE.md
├── README.md
├── update_academic.sh
└── view.sh
```

其中几乎所有内容都被存放在 content 目录下：

- accomplishments 存着 PaperCollection 这个页面的内容；
- authors 存着小组成员名单；
- home 则是主页的相关信息；
- members 主要提供 members 这个页面，内容都来自于 authors 这个文件夹；
- publications 下面是主页 Publications 下面的文章；
- talks 下面是主页 Talks 下面的内容；

还有一些比较重要的文件夹：

- docs：每次新生成的主页页面都会存进 docs 文件夹下面；它必须包含一个 CNAME 文件，指向现在的域名：zjuvag.org；
- themes：存着我修改过的 academic 主题；

生成新的静态页面并部署：`npm run deploy`
