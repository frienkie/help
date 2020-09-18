deepin的驱动问题过于致命，改刷fydeos

因为翻墙对我来说是刚需，遂摸索fydeos中翻墙的方式

fydeos的好处：pixelbook2013驱动完备，而且谷歌已经停止了pixelbook的更新，而fydeos仍然在坚持更新，本地化更好，支持chromium，安卓，linux虚拟机，微信小程序共用。

前提：v2ray for andriod提供基本的局域网连接功能，开启手机热点，配置手动代理，即可访问外网，但是很不方便

最简单的方式：chrome浏览器插件中有ss客户端，但是我的机场已经放弃了ss以及ssr，不可行

经过一番查询，得知：1.v2ray 和kitsunebi 安卓的安装包均支持andeiod x86（chromeos仅支持andriod x86应用）

2.新版chromeos中安卓容器代理设置已经和chromium共用

（其实这个时候可以直接网页下载apk安装包了）

?> kitsunebi下载项目：https://github.com/eycorsican/kitsunebi-android/releases

然后考虑通过google play下载，但是原始fydeos阉割了谷歌套件，不过留了后门，通过open Gapps完成安装

打开google play下载v2ray，然后。。。。打开代理应用就崩溃，原因未知

所幸使用clash 和kitsunebi没有问题，成功设置为系统代理，完成。

另外不知什么原因，google play下载等待时间额外漫长

也尝试过在linux容器中安装v2ray核心实现linux虚拟机中翻墙，失败，流量没有走代理，应该有什么原因，但是我实在搞不懂linux这方面的设置，再加上chromeos中linux虚拟机没有图形界面，只有终端，对于我来说实在太难了。
