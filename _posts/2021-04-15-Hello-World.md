---
title: Hello World!
tags: HelloWorld!
show_edit_on_github: false
show_subscribe: false
article_header:
  type: overlay
  background_image:
    gradient: 'linear-gradient(135deg, rgba(34, 139, 87 , .4), rgba(139, 34, 139, .4))'
    src: /assets/images/HelloWorld.jpg
---

<!--more-->
经过大概一个下午，我的github博客终于搭好了:tada:之前看[睿哥的博客](https://bot-man-jl.github.io)的时候就觉得github.io的博客看起来比CSDN有逼格多了，身为颜值控的我怎么能不试一试呢？于是今天下午摸了个鱼，找了篇[教程](https://keysaim.github.io/post/blog/2017-08-15-how-to-setup-your-github-io-blog/)搭了一下


---

总结一下大概的流程吧

1. 首先需要在自己的github目录新建一个仓库，这个仓库名是username.github.io(username是你的github用户名)
2. 向这个目录中增加静态文件，然后访问 https://username.github.io 就会看到渲染出来的效果。github默认使用Jekyll框架进行网站的构建
3. 当然，完全自己写网页是不可能的，毕竟不是所有人都懂前端，所以下一步就是挑选一款喜欢的主题:ghost:我随便搜了一些选中了现在这个TeXt
4. 安装的教程可以参照[TeXt的官网](https://tianqi.name/jekyll-TeXt-theme/docs/en/quick-start)进行，其实就是把大佬的网站拷贝一份到自己的repo，然后自己只需要更改一些配置，填充内容即可
5. 如果要本地调试的话，需要额外安装一些工具，中间遇到有一个问题是下面的代码执行报错

```ruby
bundle exec jekyll serve
```
报错信息大概是

cannot load such file -- webrick (LoadError)
{:.error}
于是我在Jekyll的github仓库issues中搜索了一下，终于找到了[解决方法](https://github.com/jekyll/jekyll/issues/8531)，输入如下命令即可：
```ruby
bundle add webrick
```
然后再执行之前的命令就可以在localhost:4000预览本地的网站效果了

---

一些有用的链接

- [TeXt Home](https://tianqi.name/jekyll-TeXt-theme/test/)
- [Emoji cheat list](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)