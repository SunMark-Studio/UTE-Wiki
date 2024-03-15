# 欢迎来到 **UTE Wiki**！

[![Gitpod Ready-to-Code](https://img.shields.io/badge/Gitpod-Ready--to--Code-brightgreen?logo=gitpod&style=flat-square)](https://github.com/SunMark-Studio/UTE-Wiki)  [![GitHub Actions](https://img.shields.io/github/actions/workflow/status/SunMark-Studio/UTE-Wiki/build.yml?style=flat-square&branch=master)](https://github.com/SunMark-Studio/UTE-Wiki/actions/workflows/build.yml)  [![Uptime Robot Status](https://img.shields.io/uptimerobot/status/m781254113-3e3bac467c64fc99eafd383e.svg?style=flat-square)](https://status.ceyase.cn/) [![QQ](https://img.shields.io/badge/QQ-UTE%20Group-blu?style=flat-square&logo=tencent-qq)](https://qm.qq.com/q/UBfHjKXzIC)  [![GitHub watchers](https://img.shields.io/github/watchers/SunMark-Studio/UTE-Wiki.svg?style=social&label=Watch)](https://github.com/SunMark-Studio/UTE-Wiki)  [![GitHub stars](https://img.shields.io/github/stars/SunMark-Studio/UTE-Wiki.svg?style=social&label=Stars)](https://github.com/SunMark-Studio/UTE-Wiki)

* * *

## 内容

Undertale 同人游戏的制作已经发展了许多年，游戏的内容越来越复杂致使难度越来越高。网上资料大多零散，没有系统的教程，因而常常需要花费大量时间探索。

**UTE Wiki** 致力于成为一个免费开放且持续更新的知识整合站点，大家可以在这里获取关于 **Undertale 粉丝游戏制作** 的有趣又实用的知识，我们准备了相关的文档和案例，为想要加入这一领域的朋友们指一条路。

本站点的灵感是从 [OI-Wiki](https://oi-wiki.org/) 上得来的，包括本 README 同样是仿照其编写。目前，**UTE Wiki** 的内容还有很多不完善的地方，大量文档没有整理，存在一些低质量页面需要修改（包括本README）。**UTE Wiki** 团队以及参与贡献的小伙伴们正在积极完善这些内容。

关于上述待完善内容，请参见 **UTE Wiki** 的 [Issues](https://github.com/SunMark-Studio/UTE-Wiki/issues)。

与此同时，**UTE Wiki** 源于社区，提倡 **知识自由**，在未来也绝不会商业化，将始终保持独立自由的性质。

* * *

## 部署

本项目目前采用 [MkDocs](https://github.com/mkdocs/mkdocs) 部署在 [ute.ceyase.cn](https://ute.ceyase.cn)。

您可以随时通过 [status.ceyase.cn](https://status.ceyase.cn) 查看 Wiki 的运行状态。

当然，也可以在本地部署。（**需要安装 Python3 和 Pipenv**）

```bash
git clone https://github.com/SunMark-Studio/UTE-Wiki.git --depth=1

cd UTE-Wiki

# 安装 mkdocs
pipenv install --pypi-mirror https://pypi.tuna.tsinghua.edu.cn/simple/

# 使用我们的自定义主题（Windows 下请使用 Git Bash 执行）
# 安装主题时将连接网络下载资源，可通过以下配置项控制下载链接
# .gitmodules:
# - url
# scripts/pre-build/install-theme-vendor.sh:
# - MATHJAX_URL
# - MATERIAL_ICONS_URL
./scripts/pre-build/install-theme.sh

# 两种方法（选其一即可）：
# 1. 运行一个本地服务器，访问 http://127.0.0.1:8000 可以查看效果
pipenv run mkdocs serve -v

# 2. 在 site 文件夹下得到静态页面
pipenv run mkdocs build -v

# 获取 mkdocs 的命令行工具的说明（解释了命令和参数的含义）
pipenv run mkdocs --help
```

我们现在在服务器端渲染 MathJax，如果希望实现类似效果，可以参考 [build.yml](https://github.com/SunMark-Studio/UTE-Wiki/blob/master/.github/workflows/build.yml)。（需要安装 Node.js）

### 镜像

```bash
# Gitee 码云 上的镜像仓库和 GitHub 仓库的内容相同
git clone https://gitee.com/SunMark-Studio/UTE-Wiki.git
```

### 离线版

可以使用 `gh-pages` 分支的内容

```bash
git clone https://gitee.com/SunMark-Studio/UTE-Wiki.git -b gh-pages
```

本地启动一个 http 服务器可能会更方便一些。

```bash
# 如果是 python3
python3 -m http.server
# 如果是 python2
python2 -m SimpleHTTPServer
# 有些环境下找不到名叫 python3/python2 的可执行文件，不妨运行 python 试试
```

### Docker

详见 [Docker 部署](https://oi-wiki.org/intro/docker-deploy/)

* * *

## 如何参与完善 OI Wiki

我们非常欢迎你为 **OI Wiki** 编写内容，将自己的所学所得与大家分享。

具体的贡献方式在 [如何参与](https://oi-wiki.org/intro/htc/)。

* * *

## 版权声明

<a rel="license" href="https://creativecommons.org/licenses/by-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />除特别注明外，项目中除了代码部分均采用<a rel="license" href="https://creativecommons.org/licenses/by-sa/4.0/deed.zh">(Creative Commons BY-SA 4.0) 知识共享署名 - 相同方式共享 4.0 国际许可协议</a>及附加的 [The Star And Thank Author License](https://github.com/zTrix/sata-license) 进行许可。

换言之，使用过程中您可以自由地共享、演绎，但是必须署名、以相同方式共享、分享时没有附加限制，

而且应该为 GitHub 仓库点赞（Star）。

而如果你想要引用这个 GitHub 仓库，可以使用如下的 bibtex：

    @misc{oiwiki,
      author = {OI Wiki Team},
      title = {OI Wiki},
      year = {2016},
      publisher = {GitHub},
      journal = {GitHub Repository},
      howpublished = {\url{https://github.com/SunMark-Studio/UTE-Wiki}},
    }

* * *

## 鸣谢

本项目受 [CTF Wiki](https://ctf-wiki.org/) 的启发，在编写过程中参考了诸多资料，在此一并致谢。

非常感谢一起完善 **OI Wiki** 的 [小伙伴们](https://github.com/SunMark-Studio/UTE-Wiki/graphs/contributors) 和为 **OI Wiki** 捐赠的 [朋友们](https://oi-wiki.org/intro/thanks/)！

<a href="https://github.com/SunMark-Studio/UTE-Wiki/graphs/contributors"><img src="https://opencollective.com/oi-wiki/contributors.svg?width=890&button=false" /></a>

特别感谢 [24OI](https://github.com/24OI) 的朋友们的大力支持！

<!-- <img src='https://i.loli.net/2018/12/07/5c0a6e4c31b30.png' alt='QVQNetWork' width=233>
鸣谢 QVQNetwork 赞助的服务器。 -->

感谢 北大算协 和 Hulu 的支持！

![](https://assets.pcmag.com/media/images/560767-hulu.png?width=333&height=245)