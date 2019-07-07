---
title: Shell系列文章
p: shell/index.md
date: 2019-07-06 17:37:29
tags: Shell
categories: Shell
top: True
---


<a name="blogshell"></a><a name="blogshell1"></a>
# Shell 脚本、bash 特性系列

我在学习 shell 和 bash 时，遇到了非常多的问题，网上的答案和总结总是不尽人意，于是下决心大致阅览了一遍 man bash，不仅总结出了不少结论，当遇到问题时也知道是哪类问题 (很多时候还真不知道)，哪里找答案，受益极大。所以个人建议，如有关于 shell 和 bash 方面的问题时，先从 man bash 中获取答案。

bash 最新英文手册：[手册](https://www.gnu.org/software/bash/manual/bashref.html)  
bash 4.0 中文手册：[下载](https://files.cnblogs.com/files/f-ck-need-u/Bash4.0%E5%8F%82%E8%80%83%E6%96%87%E6%A1%A3.pdf)

该 bash 中文手册翻译的挺好，但有些地方遗漏了内容，某些地方也遗漏了单词，而且毕竟是 4.0 版，和正在使用的 man bash 有些地方不同 (不少地方)，因此有疑问时建议中英文对照。

强烈建议：**子 shell 和执行环境的概念贯穿整个 shell，当予以最高程度的关注和重视。特别是在 shell 脚本出现 "意料之外" 又很难排查的问题时，极大可能是因为 shell 的环境问题。那些 shell 编程的书籍，只适合入门，学 shell 脚本的 "形"，不适合深入。如果有时间，建议有基础后阅读 man bash 来学 shell 的 "神"。**

<table>
    <tbody>
        <tr>
            <td>
                <ul>
                    <li>1.<a href="http://www.cnblogs.com/f-ck-need-u/p/5915048.html" target="_blank">SHELL 脚本
                            -- 简介</a></li>
                    <li>2.<a href="http://www.cnblogs.com/f-ck-need-u/p/5915076.html" target="_blank">SHELL 脚本
                            --echo 和 printf 打印输出</a></li>
                    <li>3.<a href="http://www.cnblogs.com/f-ck-need-u/p/5915106.html" target="_blank">Bash 特性
                            -- 多命令逻辑执行顺序</a></li>
                    <li>4.<a href="http://www.cnblogs.com/f-ck-need-u/p/7229381.html" target="_blank">Bash 特性
                            -- 变量 (基础)</a></li>
                    <li>5.<a href="http://www.cnblogs.com/f-ck-need-u/p/7417651.html" target="_blank">Bash 特性 -
                            bash 环境配置流程</a> (精)</li>
                    <li>6.<a href="http://www.cnblogs.com/f-ck-need-u/p/7231870.html" target="_blank">SHELL 脚本
                            -- 数学运算和 bc 命令</a></li>
                    <li>7.<a href="http://www.cnblogs.com/f-ck-need-u/p/7231832.html" target="_blank">SHELL 脚本
                            --expr 命令全解</a> (精)</li>
                    <li>8.<a href="http://www.cnblogs.com/f-ck-need-u/p/7325378.html" target="_blank">Bash 特性
                            -- 管道和重定向基础</a></li>
                    <li>9.<a href="http://www.cnblogs.com/f-ck-need-u/p/7326254.html" target="_blank">Bash 特性
                            --shell 数组基础</a></li>
                    <li>10.<a href="http://www.cnblogs.com/f-ck-need-u/p/7385133.html" target="_blank">Bash 特性
                            -- 别名 alias(通过 alias 让 rm 更安全)</a>(精)</li>
                    <li>11.<a href="http://www.cnblogs.com/f-ck-need-u/p/7401591.html" target="_blank">Bash 特性
                            -- 命令替换和命令组合</a></li>
                    <li>12.<a href="http://www.cnblogs.com/f-ck-need-u/p/7426371.html" target="_blank">Bash 特性
                            --shell 解析命令行的过程以及 eval 命令</a> (精)</li>
                    <li>13.<a href="http://www.cnblogs.com/f-ck-need-u/p/8454364.html" target="_blank">Bash 特性
                            --$ 后加引号 ($"string" 和 $'string')</a></li>
                    <li>14.<a href="http://www.cnblogs.com/f-ck-need-u/p/7454174.html" target="_blank">Bash 特性
                            --trap 捕捉信号方法论</a> (精)</li>
                    <li>15.<a href="http://www.cnblogs.com/f-ck-need-u/p/8727401.html" target="_blank">Bash 特性
                            -- 彻底搞懂 shell 的高级 I/O 重定向</a> (精)</li>
                </ul>
            </td>
            <td>
                <ul>
                    <li>16.<a href="http://www.cnblogs.com/f-ck-need-u/p/7402137.html" target="_blank">Bash 特性
                            --IFS 简单说明</a></li>
                    <li>17.<a href="http://www.cnblogs.com/f-ck-need-u/p/7402149.html" target="_blank">SHELL 脚本
                            --read 命令</a></li>
                    <li>18.<a href="http://www.cnblogs.com/f-ck-need-u/p/7427262.html" target="_blank">SHELL 脚本
                            --date、sleep、usleep 命令</a></li>
                    <li>19.<a href="http://www.cnblogs.com/f-ck-need-u/p/7427357.html" target="_blank">Bash 特性
                            --test、[]、[[]] 命令</a></li>
                    <li>20.<a href="http://www.cnblogs.com/f-ck-need-u/p/7429462.html" target="_blank">Bash 特性
                            --shell 的编程结构体</a> (精)</li>
                    <li>21.<a href="http://www.cnblogs.com/f-ck-need-u/p/7431578.html" target="_blank">Bash 特性
                            --while 循环的陷阱</a></li>
                    <li>22.<a href="http://www.cnblogs.com/f-ck-need-u/p/7521506.html" target="_blank">SHELL 脚本
                            --tr 命令用法和特性全解</a></li>
                    <li>23.<a href="http://www.cnblogs.com/f-ck-need-u/p/7521357.html.html" target="_blank">SHELL
                            脚本 --cut 命令</a></li>
                    <li>24.<a href="http://www.cnblogs.com/f-ck-need-u/p/7442886.html" target="_blank">SHELL 脚本
                            -- 玩透 sort 命令</a> (精)</li>
                    <li>25.<a href="http://www.cnblogs.com/f-ck-need-u/p/7439878.html" target="_blank">SHELL 脚本
                            --sort 命令中文手册</a></li>
                    <li>26.<a href="http://www.cnblogs.com/f-ck-need-u/p/7454597.html" target="_blank">SHELL 脚本
                            --uniq 命令</a></li>
                    <li>27.<a href="http://www.cnblogs.com/f-ck-need-u/p/7454621.html" target="_blank">SHELL 脚本
                            --seq 命令</a></li>
                    <li>28.<a href="http://www.cnblogs.com/f-ck-need-u/p/7518142.html" target="_blank">SHELL 脚本
                            --functions 文件详细分析和说明</a> (精)</li>
                    <li>29.<a href="http://www.cnblogs.com/f-ck-need-u/p/7524401.html" target="_blank">SHELL 脚本
                            -- 如何写 SysV 服务管理脚本</a> (精)</li>
                </ul>
            </td>
        </tr>
        <tr>
            <th colspan="2">子shell、bash内置命令特殊性、后台任务的本质三部曲</th>
        </tr>
        <tr>
            <td colspan="2">
                <ul>
                    <li>1.<a href="https://www.cnblogs.com/f-ck-need-u/p/9183819.html" target="_blank">bash
                            内置命令的特殊性，后台任务的 "本质"</a>(精)</li>
                    <li>2. <a href="http://www.cnblogs.com/f-ck-need-u/p/7446194.html" target="_blank">什么时候进入子
                            shell</a>(精)</li>
                    <li>3.<a href="http://www.cnblogs.com/f-ck-need-u/p/8661501.html" target="_blank">shell
                            脚本技巧：如何让 shell 脚本自杀 + bash 内置命令的特殊性</a> (精)</li>
                </ul>
            </td>
        </tr>
        <tr>
            <th>find &amp; xargs &amp; grep &amp; awk</th>
            <th>sed(pdf 版：<a href="http://down.51cto.com/data/2444639" target="_blank">玩透 sed：探究 sed 原理. pdf</a></th>
        </tr>
        <tr>
            <td>
                <ul>
                    <li>1.<a href="https://www.cnblogs.com/f-ck-need-u/p/10704754.html" target="_blank">Linux
                            find 常用用法示例 (精)</a></li>
                    <li>2.<a href="https://www.cnblogs.com/f-ck-need-u/p/6995529.html" target="_blank">Linux
                            find 运行机制详解 (精)</a></li>
                    <li>3.<a href="https://www.cnblogs.com/f-ck-need-u/p/5925923.html" target="_blank">xargs
                            原理剖析和用法详解 (精)</a></li>
                    <li>4.<a href="https://www.cnblogs.com/f-ck-need-u/p/7462706.html" target="_blank">grep
                            命令中文手册</a> (精)</li>
                    <li>5.<a href="https://www.cnblogs.com/f-ck-need-u/p/7509812.html" target="_blank">awk
                            知识点总结</a> (精)</li>
                    <li>6. <a href="https://www.cnblogs.com/f-ck-need-u/p/9621130.html" target="_blank">基础正则表达式</a>
                        (精)</li>
                    <li>7.<a href="https://www.cnblogs.com/f-ck-need-u/p/9648439.html" target="_blank">Perl
                            正则表达式超详细教程</a> (精)</li>
                    <li>8.<a href="https://www.cnblogs.com/f-ck-need-u/p/7684762.html" target="_blank">pcre
                            和正则表达式的误点</a></li>
                </ul>
            </td>
            <td><a name="sed+awk"></a>
                <ul>
                    <li>1.<a href="https://www.cnblogs.com/f-ck-need-u/p/7499471.html" target="_blank">sed
                            从入门到深入的使用心得</a></li>
                    <li>2.<a href="https://www.cnblogs.com/f-ck-need-u/p/7488469.html" target="_blank">sed 修炼系列
                            (一)：花拳绣腿之入门篇</a> (精)</li>
                    <li>3.<a href="https://www.cnblogs.com/f-ck-need-u/p/7478188.html" target="_blank">sed 修炼系列
                            (二)：武功心法 (info sed 翻译 + 注解)</a>(精)</li>
                    <li>4.<a href="https://www.cnblogs.com/f-ck-need-u/p/7496916.html" target="_blank">sed 修炼系列
                            (三)：sed 高级应用之窗口滑动技术</a> (精)</li>
                    <li>5.<a href="https://www.cnblogs.com/f-ck-need-u/p/7499309.html" target="_blank">sed 修炼系列
                            (四)：sed 中的疑难杂症</a> (精)</li>
                    <li>6.<a href="https://www.cnblogs.com/f-ck-need-u/p/8506501.html" target="_blank">sed
                            删除拼音的音调</a></li>
                    <li>7.<a href="https://www.cnblogs.com/f-ck-need-u/p/8849371.html" target="_blank">sed 示例：从
                            a 文件判断是否删除 b 文件中的行</a></li>
                </ul>
            </td>
        </tr>
        <tr>
            <td colspan="2">
                <p><strong>一些脚本示例和技巧：</strong></p>
                <ul>
                    <li>1.<a href="https://www.cnblogs.com/f-ck-need-u/p/8785561.html" target="_blank">shell
                            脚本技巧：判断 ssh 远程命令是否执行结束</a></li>
                    <li>2.<a href="https://www.cnblogs.com/f-ck-need-u/p/9746985.html" target="_blank">shell
                            脚本技巧：mapfile 读取文件内容保存到数组中</a></li>
                    <li>3.<a href="https://www.cnblogs.com/f-ck-need-u/p/9749882.html" target="_blank">shell
                            脚本技巧：tee 的花式用法和 pee</a></li>
                    <li>4.<a href="https://www.cnblogs.com/f-ck-need-u/p/9758075.html" target="_blank">shell
                            脚本技巧：getopt 设计 shell 脚本选项</a> (精)</li>
                    <li>-------------------------------------------------------</li>
                    <li>1.<a href="https://www.cnblogs.com/f-ck-need-u/p/7426987.html" target="_blank">shell
                            脚本示例：计算毫秒级、微秒级时间差</a></li>
                    <li>2.<a href="https://www.cnblogs.com/f-ck-need-u/p/7430259.html" target="_blank">shell
                            脚本示例：批量比较多个文件的内容是否相同</a></li>
                    <li>3.<a href="https://www.cnblogs.com/f-ck-need-u/p/7542210.html" target="_blank">shell
                            脚本示例：expect 实现 scp/ssh-copy-id 非交互</a></li>
                    <li>4.<a href="https://www.cnblogs.com/f-ck-need-u/p/9987052.html" target="_blank">shell
                            脚本示例：shell 脚本动画小工具 (shell 版和 perl 版)</a></li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>

<a name="blogparallel"></a>
# shell 高效率处理文本

- 1.[dd、split 和 csplit 命令](https://www.cnblogs.com/f-ck-need-u/p/7454671.html)
- 2.[shell 高效处理文本 (1)：xargs 并行处理](https://www.cnblogs.com/f-ck-need-u/p/9752365.html) (精)
- 3.GNU Parallel 6666666666






