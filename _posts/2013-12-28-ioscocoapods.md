---
layout: post
title: "iOS开发之Cocoapods包管理工具"
description: "Cocoapods包管理工具"
category: "iOS"
tags: [cocoapods]
---
{% include JB/setup %}

    iOS开发中经常用到第三方库，Cocoapods能够像ruby gems一样让你方便的实现第三方库的管理，自动为你解决包的依耐问题，免去手动添加class，framework的烦恼。
    
****
**安装(最好把本地ruby版本升级为较新的稳定版本)**
{% highlight bash %}
sudo gem install cocoapods
pod setup
{% endhighlight %}

#####使用
+ 在项目文件夹下新建一个文件:Podfile
{% highlight bash %}
cd /path/to/your/project 
vim Podfile 
{% endhighlight %}

+ 向 Podfile 加入需要的库,如:
{% highlight bash %}
platform :ios, '6.1'
pod 'AFNetworking', '~> 1.3.2' # http请求
{% endhighlight %}

+ 安装
{% highlight bash %}
pod install
{% endhighlight %}

+ 安装完毕后，Finder打开项目所在目录，以后需通过your_project_name.xcworkspace 打开项目。

+ 查找第三方cocoapods包
{% highlight bash %}
pod search your_search_lib_name
{% endhighlight %}
**用过的第三方库**
{% highlight bash %}
pod 'MMDrawerController', '~> 0.4.0' # view三屏切换
pod 'JSAnimatedImagesView', '~> 1.0.0' # 图片切换动画
pod 'AFNetworking', '~> 1.3.2' # http请求
pod 'SDWebImage', '~> 3.5' # 图片异步加载
pod 'MMProgressHUD', '~> 0.2.0' # 信息提示框
pod 'RATreeView', '~> 0.0.5' # 层级菜单tree
pod 'Reachability', '~> 3.1.1' # 网络是可用性检测
{% endhighlight %}