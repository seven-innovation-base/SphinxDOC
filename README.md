# 关于文档

[![Documentation Status](https://readthedocs.org/projects/seveninnovationbasedoc/badge/?version=latest)](https://seveninnovationbasedoc.readthedocs.io/zh_CN/latest/?badge=latest) ![GitHub](https://img.shields.io/github/license/seven-innovation-base/SphinxDOC?color=blue) ![GitHub issues](https://img.shields.io/github/issues/seven-innovation-base/SphinxDOC) ![GitHub last commit](https://img.shields.io/github/last-commit/seven-innovation-base/SphinxDOC?color=red) <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)<!-- ALL-CONTRIBUTORS-BADGE:END -->

&ensp;&ensp;本文档描述了一个伟大组织的传奇（不接受反驳~。本文档基于伟大的Sphinx项目构建，使用ReadtheDocs进行文档托管，所使用的文本标记（Markup）语言为reStructuredText + Markdown。文档使用的主题是[sphinx-rtd-theme](https://pypi.org/project/sphinx-rtd-theme/)

&ensp;&ensp;如果你想参与编辑可以先 fork 本仓库，编辑完成后再向我们提交 `pr` 。

&ensp;&ensp;由于本文档的写作基于[reStructuredText](https://zh-sphinx-doc.readthedocs.io/en/latest/rest.html)标记语言，如果你熟悉[Markdown](https://daringfireball.net/projects/markdown/syntax)，可以使用 [pandoc](https://pandoc.org/try/)进行格式转换。

## 文档的构建与写作

由于本文档基于[Spinx](https://www.sphinx.org.cn/index.html)，所以你需要安装Python的相关环境，建议使用[Pipenv](https://github.com/pypa/pipenv)进行环境管理。

- 如果你之前并未参与编辑，请先clone本项目到本地进行编辑

```bash
git clone https://github.com/seven-innovation-base/SphinxDOC
```

- 如果你之间已经clone过本项目，请先拉取更新再编辑

如果你直接clone了本项目的代码仓库，可以使用`git pull`进行拉取更新，如果你先`fork`到了自己的仓库而且clone到你本地的是你自己的仓库，那么可以编辑本地项目的`.git/config`（如果你使用的是windows系统，.git目录会默认隐藏）,增加如下配置

```bash
[remote "origin"]
	url = https://github.com/seven-innovation-base/SpinxDOC
	fetch = +refs/heads/*:refs/remotes/origin/*
```

然后使用`git pull`拉取更新

1. 如果你使用pip管理环境

```python
pip install spinx sphinx_rtd_theme
```

2. 如果你使用pipenv管理开发环境，那么你需要先cd到本文档的工程目录下，再使用以下命令安装相关依赖

```
# 安装pipenv
pip install pipenv
# 激活虚拟环境
pipenv shell
# 安装依赖
pipenv install
```

以上操作完成后，就可以编辑`*.rst`文件进行文档写作了，如果你想优化文档结构，请先阅读[Spinx文档](https://www.sphinx.org.cn/usage/quickstart.html)


如果你已经编辑完成，请先使用`make html`构建文档进行预览(构建好页面位于_build目录中)，如果检查无误再`push`到Github并向我么提交pr

## 感谢以下小伙伴的付出 ✨

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://github.com/798795982"><img src="https://avatars2.githubusercontent.com/u/40200101?v=4" width="100px;" alt=""/><br /><sub><b>GrayHat</b></sub></a><br /><a href="https://github.com/seven-innovation-base/SphinxDOC/commits?author=798795982" title="Code">💻</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

## LICENSE

Apache-2.0 © Seven Innovation base, see the [license](/LICENSE) for more details.