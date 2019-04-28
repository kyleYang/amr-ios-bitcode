# opencore-amr_for_iOS

## 新工程需要将acc转码成amr跟Android互通，由于不想关掉bitcode 搜索了很多的 opencore-arm 的库，都没有bitcode版本的，从 https://github.com/chuliangliang/opencore-amr-iOS 下载了最新的版本，但是不知道怎么总是编译不过，后在 https://my.oschina.net/u/3358032/blog/860210 搜索到了其他的编译 shell， 对shell也不是很熟，勉强看懂一点，增加了新的架构 arm64e

iOS编译生成opencore-amr类库（libopencore-amrnb.a libopencore-amrwb.a）

通过脚本编译 iOS opencore-amr类库

支持的cpu指令集: i386 x86_64 armv7 armv7s arm64 arm64e

支持bitcode: 支持bitcode

编译使用步骤:

1、将下载的文件 opencore-amr-0.1.5.tar 解压。

2、将 build_ios.sh 拷贝到 opencore-amr-0.1.5 文件夹下

3、打开命令行工具 进入到 __"opencore-amr-0.1.5"__ 目录下

4、执行命令 "./build_ios.sh",等待几分钟即可完成编译

直接使用步骤：
将文件夹中的 include 和 lib 拷贝至工程目录下，添加进去
