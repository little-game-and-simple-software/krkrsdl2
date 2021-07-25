# Kirikiri SDL2

Kirikiri SDL2 是 [Kirikiri Z](https://krkrz.github.io/)的一部分，可以运行在支持SDL2的平台上[SDL2](https://www.libsdl.org/), 比如macOS and Linux.  

这个程序可以与KAG（Kirikiri冒险游戏）3的修改版本一起使用。

有关详细信息，请参阅以下位置：https://github.com/krkrsdl2/kag3 

Kirikiri SDL2也可以编译为[WebAssembly](https://webassembly.org/)使用[Emscripten](https://emscripten.org/).  
可在web浏览器中播放的演示项目可在以下位置获得：https://krkrsdl2.github.io/krkrsdl2/

## 下载

The following builds are automatically built from the latest source code by Github Actions.  

* [Web build](https://github.com/krkrsdl2/krkrsdl2/releases/download/latest/krkrsdl2-web.zip)
* [macOS build](https://github.com/krkrsdl2/krkrsdl2/releases/download/latest/krkrsdl2-macos.zip)
* [macOS Application Bundle build](https://github.com/krkrsdl2/krkrsdl2/releases/download/latest/krkrsdl2-macos-appbundle.zip)
* [Ubuntu build](https://github.com/krkrsdl2/krkrsdl2/releases/download/latest/krkrsdl2-ubuntu.zip)

## 用法

要使用该程序，请在与“startup.tjs”相同的目录下的命令行中执行它：
```bash
/path/to/krkrsdl2
```

可以在命令行上指定启动目录或存档：
```bash
/path/to/krkrsdl2 /path/to/startup/directory
```

可以在命令行上指定命令行参数：
```bash
/path/to/krkrsdl2 -drawthread=4
```

对于web版本，请放置web版本中的文件和[Releaser]创建的“data.xp3”(https://krkrz.github.io/krkr2doc/kr2doc/contents/Releaser.html)到web服务器上。完成后，可以从web浏览器访问该项目。

## Cloning


```bash
git clone --recursive https://github.com/krkrsdl2/krkrsdl2
```
如果不使用上面的确切命令，源文件将丢失，因为项目使用Git子模块。

## Building

这个项目可以通过介子构建系统来构建。
有关系统的详细信息，请访问以下位置：https://mesonbuild.com/

介子工具链文件可用于交叉编译到不同的平台，例如使用[Emscripten](https://emscripten.org/).  
为方便起见，介子工具链文件位于以下位置：https://github.com/krkrsdl2/meson_toolchains

## Running

一旦你build了这个项目，把目录改成一个包含“startup.tjs”的目录。
 `/path/to/krkrsdl2`  

##原项目

此项目的代码基于以下项目：
* [Kirikiri 2](https://github.com/krkrz/krkr2)
* [Kirikiri Z](https://github.com/krkrz/krkrz) dev_multi_platform branch
* [KAGParser](https://github.com/krkrz/KAGParser)
* [SamplePlugin](https://github.com/krkrz/SamplePlugin)
* [wuvorbis](https://github.com/krkrz/wuvorbis)
* [ncbind](https://github.com/wtnbgo/ncbind)
* [fstat](https://github.com/wtnbgo/fstat)
* [json](https://github.com/wtnbgo/json)
* [varfile](https://github.com/wtnbgo/varfile)
* [simde](https://github.com/simd-everywhere/simde)
* [SDL](https://github.com/libsdl-org/SDL)
* [krglhwebp](https://github.com/uyjulian/krglhwebp)

## IRC Channel

Kirikiri SDL2项目的成员可以在libera.chat上的[krkrsdl2频道]中找到(https://libera.chat/).

## License

Kirikiri SDL2源代码（在'src'目录中）是根据MIT许可证授权的。有关详细信息，请阅读“许可证”。
此项目包含第三方组件。有关详细信息，请查看每个组件中的许可证文件。