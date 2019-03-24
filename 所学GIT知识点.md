# 我近段时间所学到的有关计算机的知识

首先，有的就是Markdown的一些相关的用法，通过一定的学习知道这个语言和.txt文件有一定的相似之处，不过现在的这个版本好像要比之前或者是基础教程中讲的东西有一些的不一致，一些设置可以直接通过上方的文件栏就可以对相应的字进行调整，相较于Windows自带的记事本来说，这种文件的排版会更轻松也会更好看一些，而其中的有一部分代码和HTML的有一些相似，看过网上的资料有的说“&”在HTML中和本软件中的东西不一样，或者说TYPORA中的用法更为简单，会自动的转化。

序列表分为有序和无序的，除了123之类编码的都是无序。另外，如果编号错了也会自动的矫正。

> 有关的Markdown的基础实践教程 [参考](https://www.jianshu.com/p/335db5716248)

> 该网站最好用IE打开，应为Microsoft Edge和火狐都会提示是危险网站！！

其次，就是Git这个库，以及有关的Github这个网页的库。

Git：首先有版本库，又可以叫做仓库（目录）。这个目录中的文件都可以被Git管理，每个文件的修改还有删除Git都可以跟踪——可以追踪历史纪录，也可以还原。其中一些代码的作用如图：![图片](D:\GIT\markdown图片\QQ图片20190314232710.png)上面两个就是常用的管理这个文件库的语句。其中的$ git init命令可以把这个目录变成Git可以管理的仓库。<font color=red>**这个文件是.git文件格式结尾，这个目录是Git来跟踪管理版本库的，没事千万不要手动修改这个目录里面的文件，不然改乱了，就把Git仓库给破坏了。**</font>

$ git add+文件名与它的后缀可以自动将这个文件转入Git的库的目录中（执行上述的代码后如果<font color=red>没有任何显示就表示添加成功</font>。如果显示did not match any files时 ，实际上是没有把文件放入相应的文件放入版本库的文件夹下，后再使用$ git add来添加文件,有时也可以用<font color=green>**$ git status**</font>来<font color=green>**查看状态**</font>，<font color=red>touch+文件名</font>意思是建立一个新文件）。$ git commit -m"对这次修改的描述"，该描述最好写上，方便以后查询修改；该命令执行成功后会显示（）file changed，（）insertions（+），（）deletions（-），分别是<font color=red>（）个文件被改动</font>，<font color=red>插入</font>了（）行内容，<font color=red>删减</font>了（）行内容。$ git log是用于查询修改的记录的，相当与<font color=red>查询历史纪录</font>>的操作，方便以后的查寻修改之前的版本，如果不小心删除了还可以再恢复文件。

文件的恢复：用到命令<font color=red>$ git reset --hard HEAD</font>,在Git中，用<font color=green>**HEAD**</font>表示当前版本，也就是最新的提交的版本。上一个版本就是<font color=blue>**HEAD^**</font>，上上一个版本就是<font color=blue>**HEAD^^**</font>，当然往上100个版本写100个`^`比较容易数不过来，所以写成<font color=red>**HEAD~100**</font>。

>![](D:\GIT\markdown图片\未解难题1.png)
>
>![未解难题我2](D:\GIT\markdown图片\未解难题我2.png)

解决办法：（前提：<font color=red>以对文件进行过修改</font>）

![](D:\GIT\markdown图片\解决方案1~2.png)

工作区与版本库：![](D:\GIT\0.jpeg)

> git add的文件添加到暂存区（stage），git commit是提交文件到master中,可以简单的理解为提交的文件修改通通放在stage中，再一次性提交所有的修改，

