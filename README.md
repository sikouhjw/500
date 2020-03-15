# 重排《高等数学证明题500例》

排版规则：

- 中西文之间留空格
- 文字与数学公式之间留空格，如 `求极限 $\lim_{n \to \infty} x_n$`，例外是与中文标点相接时
- 数学公式中留适当的空格，如 `\sin x \lim_{n \to \infty} \frac{\sin x}{\sqrt[n]{x \ln x}}`
- 列表：
  - 题目用 `\begin{ti} content \end{ti}` 环境
  - 小题 `(1)(2)` 用 `\begin{xiaoti} content \end{xiaoti}` 环境
  - 带圈数字 `①②` 用二次嵌套的小题环境 `\begin{xiaoti} content \begin{xiaoti} content \end{xiaoti} \end{xiaoti}`

- 不要用 `\dfrac` 等破坏风格一致性的命令
- 括号尽量用 `\bigl \bigr` 之类的，而不是 `\left \right`，可能会导致换行不成功问题
- 逗号的使用
  - 文字中用中文逗号 `，`
  - 文字与数学公式中，用中文逗号 `，`，如：`求这个极限，$\lim_{n \to \infty}$`
  - 数学公式与数学公式之间，用西文逗号 `,`，如：`($n=1$, $2$, $3$, $\cdots$)`，像这种列举的地方，像例子一样输入，方便换行

- 括号的使用，文字中使用中文括号`（）`，数学公式中使用西文括号`()`，即使里面包含了中文
- 句号的使用，文字中使用中文句号 `。`，数学公式中使用西文逗号 `.`
- 其它中西文符号使用参考以上几点，也可以看我的代码
- 数学公式中的乘号，用 `\cdot`，省略号用 `\cdots`
- 符号不会输出，去查 `lshort-zh`
- 数学公式中，如果有横向间距，用 `\quad`
- 如果有额外的宏包加载 / 其他导言区设置，请在合并的时候交流后再选择保留哪个
- **别调格式**

- 题目 / 小题如果带了 `*` 星号，在该位置使用命令 `\xing{}`

git 使用：

1. fork 下来，切换到对应的分支，在分支上修改，push 到分支上
2. 重排完负责的，先 push 到对于分支，再 merge 到 master

不会的操作就去查 [https://gitee.com/all-about-git](https://gitee.com/all-about-git)