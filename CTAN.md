CTAN (The Comprehensive TeX Archive Network) 镜像源可以使用 TeX Live 管理器 `tlmgr` 更改。

在命令行中执行

```bash
tlmgr option repository https://mirrors.pku.edu.cn/ctan/systems/texlive/tlnet
```


即可永久更改镜像源。

如果只需要临时切换，可以用如下命令：

```bash
tlmgr update --all --repository https://mirrors.pku.edu.cn/ctan/systems/texlive/tlnet
```


其中的 `update --all` 指令可根据需要修改。


CTAN 同时支持 MiKTeX 发行版，该发行版支持 Windows、Linux 和 macOS。

镜像使用方法

MiKTeX 使用的 CTAN 镜像源可以从内置的 MiKTeX Console 图形化应用程序进行切换

1. 打开 MikTeX Console 图形应用程序；
2. 点击主界面左侧 `设置`；
3. 在设置标签栏中选择 `常规`；
4. 选择 `宏包安装`，点击更改；
5. 在选择宏包源的类型中选择 `远程宏包存储库(互联网)`（默认选中）；
6. 点击 `Next`；
7. 在弹出的界面中找到并选中 `mirrors.pku.edu.cn`；
8. 点击 `Finis` 完成设置；

MiKTeX Console 同时支持命令行管理，也可以在命令行中执行如下命令：

```bash
mpm --set-repository=https://mirrors.pku.edu.cn/ctan/systems/win32/miktex/tm/packages
```
