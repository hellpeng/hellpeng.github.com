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

**通过pygments使代码高亮**
> 需要在配置文件_config.yml设置参数: pygments: true
<pre><code>生成pygments.css样式文件
cd path_to_project
pygmentize -f html -S default > pygments.css
然后在_layout模板中引用该样式文件
</code></pre>
<pre><code> {% highlight ruby %}
def foo
  puts 'foo'
end
{% endhighlight %}
</code></pre>
highlight参数: ruby , objc

