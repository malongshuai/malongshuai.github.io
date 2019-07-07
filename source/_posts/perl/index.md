---
title: Perl系列文章
p: perl/index.md
date: 2019-07-06 17:37:29
tags: Perl
categories: Perl
top: True
---

# Perl书籍推荐

[**Perl书籍下载**](https://pan.baidu.com/s/1IcY9rA7hAz1wfczl0Lll2Q)  密码：kkqx

下面是一些我学习Perl过程中读过完整的或部分章节的觉得好的书。

- **入门级别1**：《Perl语言入门》即小骆驼  
- **入门级别2**：《Intermediate Perl》即羊驼  
- **入门后复习**：《beginning Perl》  
- **系统性学习和进阶**：《Pro Perl》（目前在读，是我整理、完善Perl的最佳书籍）  
- **Perl编码技巧**：《Perl高效编程》(英文版Effective Perl Programming)

关于《精通perl》和《Perl语言编程》（即羊驼一家和大骆驼），虽然网上评价很高，但是觉得始终不适合，或者说不适合中国人。精通Perl是作者(brian d foy)以第一人称来描述他怎么理解Perl的，Perl语言编程是Larry Wall自己编写的书籍，也许他智商太高，书中很多地方的跳跃性都非常大。

然后是某个方向的书籍，比如http客户端《perl lwp》(看了一半，作者的写作方式非常友好)、数据库操作《Programming the Perl DBI》（有中文版）。

最后，是我的这些博客，它们是我阅读这些书籍的读书笔记，更多的是我测试和补充的内容，可以免去看英文版，也免去书中的一大堆废话，老外的书，你懂的。


# Perl语言入门

本部分是《Perl语言入门 第六版》(英文书名：Learning Perl)的学习笔记，这本书是Perl家族的"小羊驼"书籍。我个人学习这本书的感觉，如果有shell基础，perl入门挺容易的。

## 入门基础

<table>
    <tbody>
        <tr>
            <td>
                <ul>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9512028.html">1.Perl 语法的基本规则</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9511844.html">2.Perl 的数值和字符串</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9511857.html">3.Perl 的变量</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9536582.html">4.Perl 中的自增、自减</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9511867.html">5.Perl 的比较操作符</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9511878.html">6.Perl 的流程控制语句</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9511936.html">7.Perl 的 undef 类型和
                            defined() 函数</a></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9511892.html">8.Perl 读取输入
                            &lt;STDIN&gt;、&lt;&gt; 和 chomp 函数</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9511949.html">9.Perl 的列表和数组</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9525098.html">10.Perl 中的 hash 类型</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9511968.html">11.Perl 的执行上下文</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9618292.html">12.Perl 分片技术</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9557517.html">13.Perl 的输出：print、say 和
                            printf</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9512313.html">14.Perl 的子程序</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9695536.html">15.Perl 的 do 语句块结构</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9520707.html">16.Perl 的 die 和 warn 函数</a><br></li>
                </ul>
            </td>
            <td>
                <ul>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9557041.html">17.Perl 的命令行参数和 ARGV</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9568879.html">18.Perl 的 IO 操作 (1)：文件句柄</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9570654.html">19.Perl 的 IO 操作
                            (2)：更多文件句柄模式</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9568468.html">20.Perl 文件句柄相关的常见变量</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9589419.html">21.Perl 文件测试操作和 stat 函数</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9609676.html">22.Perl 文件名通配和文件查找</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9601928.html">23.Perl 文件、目录常用操作</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9609349.html">24.Perl 复制、移动、重命名文件 / 目录</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9611098.html">25.Perl 的 time、localtime 和
                            gmtime 函数</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9648439.html">26.Perl 正则表达式超详细教程</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9655273.html">27.Perl 处理数据 (一)：s
                            替换、split 和
                            join</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9655841.html">28.Perl 处理数据 (二)：tr 和 y///</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9685581.html">29.Perl 模块管理</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9685957.html">30.Perl 使用模块和 @INC</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9691714.html">31.Perl 和 OS 交互
                            (一)：system、exec 和反引号</a><br></li>
                    <li><a href="https://www.cnblogs.com/f-ck-need-u/p/9693675.html">32.Perl 和 OS 交互 (二)：fork</a><br></li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>


## 其它基础

- [1.Perl函数：字符串相关函数](https://www.cnblogs.com/f-ck-need-u/p/9666341.html)  
```
chomp, chop, chr, crypt, fc, hex, index, lc, 
lcfirst, length, oct, ord, pack, q//, qq//, 
reverse, rindex, sprintf, substr, tr///, 
uc, ucfirst, y///
```
- [2.Perl函数：列表相关函数](https://www.cnblogs.com/f-ck-need-u/p/9678875.html)  
```
grep, join, map, qw//, reverse, sort, unpack
```
- [3.Perl函数：数组和hash相关函数](https://www.cnblogs.com/f-ck-need-u/p/9680347.html)  
```
数组：each, keys, pop, push, shift, splice, unshift, values
hash：delete, each, exists, keys, values
```
- [4.List::Util模块用法详解](https://www.cnblogs.com/f-ck-need-u/p/10340230.html)   

<p><a name="blogperloneline"></a></p>

# Perl一行式程序

这部分分3部分，内容比较多，算得上是一本薄书了，所以专门加上了一个《序言》，让它看上去更像是书。

第一部分是针对没有Perl基础，但想用perl一行式命令的人，用于快速掌握学习perl一行式时所必须知道的Perl基础知识。

第二部分是perl的选项、特殊变量的收集，没有多少示例，只是它们详细的解释，专门用来做perl一行式的参考手册或者熟练后的速查手册。第一次学perl一行式的人不建议直接看这一篇文章，而是直接从后面的示例部分开始看，需要完整、详细说明的时候再回来看这篇文章中对应的内容。

第三部分是一大堆perl一行式的使用示例(分成了好几篇文章)，也是学习perl一行式的入口，前提是你已经具备了Perl基础知识。这些例子不一定都是实用的例子，只是为了抛砖引玉。这部分会针对用法来对选项、perl语句做不完整解释，如果想要知道完整的解释，看第二部分的文章。

示例部分主要来自于《Perl One-Liners》这本书，但我自己对内容进行了大量扩充，也进行了更多的解释。

- [1.序言：我为什么学Perl](https://www.cnblogs.com/f-ck-need-u/p/10217587.html)  
- [2.Perl 0基础的人学习Perl一行式必知的Perl基础](https://www.cnblogs.com/f-ck-need-u/p/10217597.html)  
- [3.perl选项、特殊变量参考手册](https://www.cnblogs.com/f-ck-need-u/p/10219326.html)
- [4.Perl一行式：处理空白符号](https://www.cnblogs.com/f-ck-need-u/p/10219742.html)
- [5.Perl一行式：处理行号和单词数](https://www.cnblogs.com/f-ck-need-u/p/10223704.html)
- [6.Perl一行式：字段处理和计算](https://www.cnblogs.com/f-ck-need-u/p/10240314.html)
- [7.Perl一行式：文本编解码、替换](https://www.cnblogs.com/f-ck-need-u/p/10243772.html)
- [8.Perl一行式：选择输出、删除的行](https://www.cnblogs.com/f-ck-need-u/p/10247059.html)



# Perl语言进阶

本部分是《Intermediate Perl 2nd》的学习笔记，这本书是骆驼家族的"羊驼"书，用于Perl的基础进阶学习。部分内容来自《Beginning Perl》，这也是一本好书。

## 引用

- [1.Perl引用入门](https://www.cnblogs.com/f-ck-need-u/p/9708263.html)  
- [2.Perl解除引用：从引用还原到数据对象](https://www.cnblogs.com/f-ck-need-u/p/9710562.html)  
- [3.Perl检查引用类型](https://www.cnblogs.com/f-ck-need-u/p/9713851.html)  
- [4.Perl匿名数组、hash和autovivification特性](https://www.cnblogs.com/f-ck-need-u/p/9718238.html)  
- [5.Perl的浅拷贝和深度拷贝](https://www.cnblogs.com/f-ck-need-u/p/9721265.html)  
- [6.Perl输出复杂数据结构：Data::Dumper,Data::Dump,Data::Printer](https://www.cnblogs.com/f-ck-need-u/p/9719282.html)  
- [7.Perl数据序列化和持久化(入门)：Storable模块](https://www.cnblogs.com/f-ck-need-u/p/9723368.html)    
- [8.Perl子程序引用和匿名子程序](https://www.cnblogs.com/f-ck-need-u/p/9733283.html)    
- [9.一文搞懂：词法作用域、动态作用域、回调函数、闭包](https://www.cnblogs.com/f-ck-need-u/p/9735955.html)    
- [10.Perl回调函数和闭包](https://www.cnblogs.com/f-ck-need-u/p/9738156.html)  
- [11.Perl文件句柄引用](https://www.cnblogs.com/f-ck-need-u/p/9740059.html)  
- [12.Perl正则表达式引用](https://www.cnblogs.com/f-ck-need-u/p/9743199.html)  
- [13.排序变换思路：施瓦茨变换](https://www.cnblogs.com/f-ck-need-u/p/9744275.html)  

## 包和模块  

- [1.Perl导入代码文件(eval、do、require)](https://www.cnblogs.com/f-ck-need-u/p/9770651.html)  
- [2.Perl包和模块(内容来自beginning perl)](https://www.cnblogs.com/f-ck-need-u/p/9779949.html)  
- [3.Perl包相关](https://www.cnblogs.com/f-ck-need-u/p/9771806.html)  
- [4.Perl特殊代码块：BEGIN、CHECK、INIT、END和UNITCHECK](https://www.cnblogs.com/f-ck-need-u/p/9780625.html)  
- [5.Perl：写POD文档](https://www.cnblogs.com/f-ck-need-u/p/9781455.html)  
- [6.Perl构建和打包自己的模块](https://www.cnblogs.com/f-ck-need-u/p/9782737.html)  

## Perl面向对象

- [1.Perl面向对象(1)：从代码复用开始](https://www.cnblogs.com/f-ck-need-u/p/9798757.html)  
- [2.Perl面向对象(2)：对象](https://www.cnblogs.com/f-ck-need-u/p/9811119.html)  
- [3.Perl面向对象(3)：解构——对象销毁](https://www.cnblogs.com/f-ck-need-u/p/9818016.html)  

**待续。。。**

# Perl进程、线程、IO

- [1.Perl信号处理](https://www.cnblogs.com/f-ck-need-u/p/10386248.html)  
- [2.Perl多进程](https://www.cnblogs.com/f-ck-need-u/p/10386933.html)  
- [3.Perl处理和收走子进程](https://www.cnblogs.com/f-ck-need-u/p/10389627.html)  
- [4.Perl进程：僵尸进程和孤儿进程](https://www.cnblogs.com/f-ck-need-u/p/10508297.html)  
- [5.Perl进程间通信](https://www.cnblogs.com/f-ck-need-u/p/10400540.html)  
- [6.Perl SysV IPC](https://www.cnblogs.com/f-ck-need-u/p/10404275.html)  
- [7.Perl线程(1)：解释器线程特性和线程管理](https://www.cnblogs.com/f-ck-need-u/p/10420910.html)  
- [8.Perl线程(2)：数据共享和线程安全](https://www.cnblogs.com/f-ck-need-u/p/10422445.html)  
- [9.Perl线程队列：Thread\:\:Queue](https://www.cnblogs.com/f-ck-need-u/p/10422293.html)  
- [10.Perl线程池](https://www.cnblogs.com/f-ck-need-u/p/10422449.html)  
- [11.Perl IO：简介和常用IO模块](https://www.cnblogs.com/f-ck-need-u/p/10442177.html)  
- [12.Perl IO：read()函数](https://www.cnblogs.com/f-ck-need-u/p/10442188.html)  
- [13.Perl IO：随机读写文件](https://www.cnblogs.com/f-ck-need-u/p/10446013.html)  
- [14.Perl IO：文件锁](https://www.cnblogs.com/f-ck-need-u/p/10447881.html)  
- [15.Perl IO：IO重定向](https://www.cnblogs.com/f-ck-need-u/p/10450299.html)  
- [16.Perl IO：操作系统层次的IO](https://www.cnblogs.com/f-ck-need-u/p/10459768.html)  

# 网络编程

- [Perl获取主机名、用户、组、网络信息](https://www.cnblogs.com/f-ck-need-u/p/10486209.html)  

# balabala

[Perl输出带颜色行号或普通输出行](https://www.cnblogs.com/f-ck-need-u/p/10791792.html)





