# Windows环境编译

## 1. 安装工具

下载如下工具，并添加相应路径至 %PATH% 环境变量。
* [git](https://git-scm.com/download/win)
* [Python 3](https://www.python.org/downloads/windows/)
* [Node.js 10.15.3](https://nodejs.org/download/release/v10.15.3/)
* [CMake](https://cmake.org/install/)
* [Visual Studio 2017](https://my.visualstudio.com/Downloads?q=visual%20studio%202017&wt.mc_id=o~msft~vscom~older-downloads) - 只需要安装VC140。

运行下面命令并安装`yarn`, `electron-builder`和`pipenv`。

```
C:\> npm install -g yarn electron-builder
C:\> pip install pipenv
```
## 2. 编译


获取代码并编译：
```
$ git clone https://github.com/QT-Wonder/kungfu.git
$ cd kungfu
$ yarn
$ yarn build
```

编译结果输出在 app/build 目录下，可执行文件在`kungfu\app\build\app\win-unpacked`，安装包在`kungfu\app\build\app`。

遇到编译问题需要完整的重新编译时，执行以下命令清理临时文件：
```
$ yarn clean
```

