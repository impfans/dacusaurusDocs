# 使用Docusaurus



## 一、安装Docusaurus

### 1. 使用npx安装

Typescript 版本

`npx create-docusaurus@latest my-website classic --typescript`



### 2.安装后项目结构

生成项目结构

```markdown
my-website
├── blog
│   ├── 2019-05-28-hola.md
│   ├── 2019-05-29-hello-world.md
│   └── 2020-05-30-welcome.md
├── docs
│   ├── doc1.md
│   ├── doc2.md
│   ├── doc3.md
│   └── mdx.md
├── src
│   ├── css
│   │   └── custom.css
│   └── pages
│       ├── styles.module.css
│       └── index.js
├── static
│   └── img
├── docusaurus.config.js
├── package.json
├── README.md
├── sidebars.js
└── yarn.lock
```



#### 结构介绍

- `/blog/`- 包含博客 Markdown 文件。如果您禁用了博客插件，您可以删除该目录，或者您可以在设置选项后更改其名称`path`。[可以在博客指南](https://docusaurus.io/docs/blog)中找到更多详细信息
- `/docs/`- 包含文档的 Markdown 文件。自定义文档侧边栏的顺序`sidebars.js`。如果您禁用了文档插件，您可以删除该目录，或者您可以在设置选项后更改其名称`path`。[可以在文档指南](https://docusaurus.io/docs/docs-introduction)中找到更多详细信息
- `/src/`非文档文件，如页面或自定义 React 组件。您不必严格地将非文档文件放在这里，但将它们放在一个集中目录下可以更容易地指定，以防您需要进行某种检查/处理
  - `/src/pages`- 此目录中的任何 JSX/TSX/MDX 文件都将转换为网站页面。[可以在页面指南](https://docusaurus.io/docs/creating-pages)中找到更多详细信息
- `/static/`- 静态目录。这里的任何内容都将被复制到最终`build`目录的根目录中
- `/docusaurus.config.js`- 包含站点配置的配置文件。这相当于`siteConfig.js`Docusaurus v1
- `/package.json`- Docusaurus 网站是一个 React 应用程序。你可以在其中安装和使用任何你喜欢的 npm 包
- `/sidebars.js`- 文档使用它来指定侧边栏中文档的顺序



### 3. 运行项目

<Tabs>

​	<TabItem value = "npm" label = "npm" default>

​		npm run start

​	</TabItem>

​	<TabItem value = "yarn" label = "yarn" default>

​		yarn run start

​	</TabItem>

</Tabs>



## 二、 配置介绍

