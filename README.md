# Proxy-Factory
This project is written in Apple Swift Language, provide an interface to switch proxy service goagent and goproxy, and some useful functions for macOS user. 

macOS user can:
1.Switch between goagent and goproxy  2.Toggle system proxy settings without require password(only once) by use SMJobless + XPC 3.Fix port confict automatically  4.Import RootCA to system 5.Update goproxy from github  6.User friendly interface to change general settings such as AppIDs, Password, Proxy Port, IP List, etc. 
(*goproxy and goagent are developed by phuslu, https://github.com/phuslu/goproxy.)

This is also a sample application of SMJobless and XPC written in Swift language. When I started this project, I could not find any SMJobless and XPC samples written in Swift on the Internet. The Apple samples are written in Objective C. In this project, the SMJobless part and helper tool are all implemented in Swift. I may upload a simplified sample with configuration explanation step by step later.

我经常用Goproxy在macOS下翻墙，使用中发现一些不便，于是在学习Swift时写一个macOS GUI客户端，打包了goproxy和goproxy，提供一些自已常用的功能：
1.一键切换goproxy和goagent, 
2.一键更改macOS系统代理设置, 切换Autoproxy PAC模式与HTTP/HTTPS模式
3.自动Kill占用端口的其他进程
4.导入RootCA
5.从Github下载更新goproxy
6.界面用来更改常见设置，如AppIDs, Password, 端口，IP List等，IP List输入框支持 |、空格、tab分隔。

因为使用SMJobless + XPC, 所以只需要在第一次启动时需要输入密码来授权安装helper tool，以后使用再也不需要密码来更改系统设置。

更新：goproxy的更新链接、添加开机自启动功能。

项目地址：https://github.com/ping99/Proxy-Factory
