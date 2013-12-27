![Hellpeng ico](http://hellpeng.github.io/favicon.ico)
### Jekyll常用命令
**主题安装**
<pre><code>rake theme:install git="https://github.com/jekyllbootstrap/theme-twitter.git"
</code></pre>

**发表文章**
<pre><code>rake post title="Hello World"
</code></pre>

**本地预览**
<pre><code>rake preview</code></pre>

**创建页面**
<pre><code>rake page name="about.md"</code></pre>

**Push到Github**
<pre><code>$ git add .
$ git commit -m "Add new content"
$ git push origin master
</code></pre>

**文章嵌入视频**
> 需要将tudou.rb/youku.rb脚本拷贝到_plugins目录下
<pre><code>优酷视频
{% youku XNjUyOTQ3NzE2 %}
{% youku XNjUyOTQ3NzE2 500 500%}
土豆视频
{% tudou 8p6gpToUHi0 %}
{% tudou 8p6gpToUHi0 500 500%}
</code></pre>