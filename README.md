# 关于文档📌

[![Documentation Status](https://readthedocs.org/projects/seveninnovationbasedoc/badge/?version=latest)](https://seveninnovationbasedoc.readthedocs.io/zh_CN/latest/?badge=latest) ![GitHub](https://img.shields.io/github/license/seven-innovation-base/SphinxDOC?color=blue) ![GitHub issues](https://img.shields.io/github/issues/seven-innovation-base/SphinxDOC) ![GitHub last commit](https://img.shields.io/github/last-commit/seven-innovation-base/SphinxDOC?color=red)  [![Netlify Status](https://api.netlify.com/api/v1/badges/020b729a-30f0-4330-8f85-c0a9bcbd90a3/deploy-status)](https://app.netlify.com/sites/vibrant-lumiere-4558d4/deploys)<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-3-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

>本文档描述了一个伟大组织的传奇（不接受反驳~😊(●'◡'●)）

本文档基于伟大的[Sphinx](http://www.sphinx-doc.org/en/master/)项目构建（你没想错，伟大的[Python](https://docs.python.org/3/)的文档就是用它整的），我们还使用了同样伟大的GitHub和[ReadtheDocs](https://docs.readthedocs.io/en/stable/index.html)进行文档自动构建和托管，文档写作所使用的文本标记（Markup）语言为reStructuredText + Markdown。文档使用了不怎么帅的主题[sphinx-rtd-theme](https://pypi.org/project/sphinx-rtd-theme/)。

**如果各位路过的大佬发现文档有写的不对或者可以改进的地方，欢迎向我们提issue和pull request，谢谢啦(●'◡'●)**

## 如何参与文档的编辑与维护✍

由于本文档基于[Sphinx](https://www.sphinx.org.cn/index.html)，而这玩意是个Python项目，所以你需要安装[Python](https://www.python.org/downloads/)的相关环境，你不需要会Python就可编辑和构建文档。文档的主要依赖（Python Packages）如下：

```
sphinx

sphinx-rtd-theme

recommonmark
```

**注意❗❗❗**：

参与维护前请先 fork 本仓库，然后基于 fork 后的仓库的 master 分支创建一个**新的分支**（名字随意），修改后提交到这个新的分支，然后基于这个分支向本仓库发送 pull request，会有人对你的 pull request 进行 review，review 通过后会合并到本仓库

如果后续想要继续参与维护，参考以下commit log的**同步流程**：

1. 添加本仓库为你 fork 后仓库的远程上游 `upstream`

```shell
git remote add upstream https://github.com/seven-innovation-base/SphinxDOC.git
# 或者
git remote add upstream git@github.com:seven-innovation-base/SphinxDOC.git
```

2. 同步远程上游 upstream 的变更

```shell
git fetch upstream
```

3. 将远程上游的变更合并到你 fork 后的仓库的 master 分支中，保证你的 master 分支永远都是最新的

```shell
git merge upstream/master
```

然后再基于 master 分支新建新的分支，提交你的变更到你所创建的新的分支，最后提交 pull request

### 一、环境配置

在开始前请先`fork`一下这个项目，再`clone`到本地（clone的是你名下的同名仓库）

我们建议你使用`virtualenv+pip`的方式管理本文档构建所依赖的环境，如果你想使用pipenv或者单纯用pip也行，方法如下：

```bash
git clone https://github.com/your_username/SphinxDOC
```

#### pip + virtualenv

```bash
# 1、转到项目目录
cd SphinxDOC
# 2、安装virtualenv
pip install virtualenv
# 3、为本项目创建虚拟环境
virtualenv venv
# 4、激活虚拟环境
cd venv/Scripts
activate
cd ../..
# 5、安装依赖
pip install -r requiremen.txt
# 6、清除之前构建好的文件
make clean
# 7、试下构建文档
make html
# 8、构建好的静态文件再_build目录下，点击index.html进行预览
```

#### pipenv

```bash
pip install pipenv

pipenv install  # 创建虚拟环境，安装依赖

pipenv shell  # 激活虚拟环境

./make clean

./make html  # 构建文档，在_build/html/index.html 预览
```

### 二、文档编辑与构建

环境搭建好后，就可以编辑`*.rst`、`*.md`文件进行文档编辑了，如果你想新增`rst`、`md`文件或优化文档结构，请先阅读[Sphinx中文文档](https://www.sphinx.org.cn/usage/quickstart.html#defining-document-structure)的文档结构的定义章节

md的格式有限，可以考虑用rst，可以一开始可以用Markdown写然后用[pandoc](https://pandoc.org/try/)将Markdown格式转换为restructText继续编辑。

如果你已经编辑完成，请先使用`make clean`清除之前构建好的静态文件，然后使用`make html`构建新文档，然后进行效果预览(构建好文件位于**_build/html**目录中)，如果没啥毛病就`push`到GitHub并向我们提交`pull request`

### 拓展阅读

- [Sphinx介绍](https://www.sphinx.org.cn/intro.html#usage)
- [文档项目信息配置](https://www.sphinx.org.cn/usage/configuration.html#project-information)
- [Sphinx Markdown支持](https://www.sphinx.org.cn/usage/markdown.html)
- [RST初级读本](https://www.sphinx.org.cn/usage/restructuredtext/basics.html)

## 感谢以下小伙伴的付出 ✨

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://github.com/798795982"><img src="https://avatars2.githubusercontent.com/u/40200101?v=4" width="100px;" alt=""/><br /><sub><b>GrayHat</b></sub></a><br /><a href="https://github.com/seven-innovation-base/SphinxDOC/commits?author=798795982" title="Code">💻</a></td>
    <td align="center"><a href="https://shansan.top"><img src="https://avatars2.githubusercontent.com/u/39296814?v=4" width="100px;" alt=""/><br /><sub><b>Mr.Ye</b></sub></a><br /><a href="https://github.com/seven-innovation-base/SphinxDOC/commits?author=yeshan333" title="Code">💻</a></td>
    <td align="center"><a href="https://mrgo123.github.io"><img src="https://avatars1.githubusercontent.com/u/53072382?v=4" width="100px;" alt=""/><br /><sub><b>yizhuang</b></sub></a><br /><a href="https://github.com/seven-innovation-base/SphinxDOC/commits?author=MrGo123" title="Documentation">📖</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

## 许可证📑

Apache-2.0 © Seven Innovation base, see the [license](/LICENSE) for more details.
