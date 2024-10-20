--- 
title: 111
date: 2024-10-20 23:45:40
---

修改玩文章,hexo s是预览,可以实时看到编译后的模样.满意了之后hexo d

最好是

```bash
hexo clean
hexo g
hexo d
```

hexo 默认只会编译新建的博客,所以要先hexo clean清除之前的缓存,然后hexo g重新生成,最后hexo d部署到GitHub上面去,g代表generate,d是deploy


出现这个INFO  Deploy done: git就是成功了

然后最好每次修改之后把这个仓库也上传到github,这样可以随时恢复之前的内容.
这个仓库里放的是源代码,hexo d会把源代码编译到public和.deploy_git子文件夹,然后把他们俩上传到gh-pages分支,但是这个子文件夹是不包括源代码的,没法追踪源代码的变化,所以要把源代码也上传,在侧边栏git那里写好message点commit和sync就好了
