# learn-vim
### vim 基础操作
* 数字 + 命令  == 多次执行该命令
* 编辑模式
    * 编辑内容
* 视图模式
    * v  行选择
    * Ctrl + v 块选择
* normal模式
    * i（insert）光标前插入
    * I 行首插入
    * o (open a line below) 插入新的下一行
    * O (open a line before) 插入新的上一行
    * a (append) 光标后追加
    * A 行尾追加 
* 快捷操作
    * Ctrl + u 删除一行
    * Ctrl + w 删除上一个单词
    * Ctrl + h 删除上一个字符
    * Ctrl + a 移动到行首
    * Ctrl + e 移动到行尾
    * Ctrl + b 向前移动
    * Ctrl + f 向后移动
    * Ctrl + [ 等于ESC键
    * gi 跳转到上一次编辑的位置
* 快速移动
    * hjkl 左下上右
    * w/W（空格符） 移动到下一个单词的开头  e/E 移动到下一个单词的结尾
    * b/B 移动到上一个单词的开头
* 行间搜索移动
    * f{char} 搜索光标之后
    * F{char} 搜索光标之前
    * ;下一个   ，上一个
* 水平移动
    * 0 移动到行首第一个字符   ^ 移动到第一个非空白字符
    * $ 移动到行尾    g_移动到行尾非空白字符
* 页面移动
    * gg 移动到文件的开头
    * G 移动到文件的结尾
    * ctrl + o 快速返回
    * H (head) 开头
    * M (Middle)中间
    * L (Lower) 结尾
    * ctrl + U 上翻页
    * ctrl + F 下翻页
    * zz 把光标行移动到屏幕中间
* 快速增删改查
    * 增加：
        * i
        * a
        * o 
    * 删除：  
        * x 删除一个字符  3x
        * daw/diw 删除一个单词
        * dd 删除一行   3dd
        * dt{char}  删除到{char}字符之前的全部
        * d0/d$
    * 修改：
        * r(replace) 替换 
        * c(change) ct{char}   
            * cw (change word) 删除一个单词
            * ct (change to)  删除到{char}字符之前的全部
        * s(substitute) 替换并插入
    * 查询：
        * / 进行向前搜索 ？ 反向搜索
        * n 向下匹配  N 向上匹配
        * (*) 向前单词匹配  （#）向后单词匹配 
* 搜索替换
    * :[range]s/{pattern/{string}/[flags]
    * range 表示范围 比如： 10,20 表示10-20行，% 表示全部
    * pattern 要替换的模式
    * string 替换后的字符串
    * flags
        * g(global) 全局范围内执行
        * c(confirm) 表示确认
        * n(number) 报告匹配次数而不替换
* 多文件操作
    * Buffer 打开一个文件的内缓存区
	* :ls 列举目前的缓冲区  :b n 跳转到第n个的缓冲区 
    * Window Buffer可视化的分隔区域
	* :vs 垂直分隔  :sp 水平分隔
	* 窗口切换: ctrl + w + h/j/k/l
    * Tab 可以组织几个Window为一个工作区		
	* :tabe filename
	* gt 切换到下一标签页
   
* 文本对象操作
    * [number]<command>[text object]
    * number 次数
    * command 命令 d(elete),c(hange),y(ank)
    * text object 文本对象，单词w,句子s,段落p
* 复制粘贴与寄存器
    * normal模式
        * y(ank)复制  p(ut)粘贴  d(elete)剪切
        * 使用v选中某块区域，再使用p粘贴
        * yiw 复制一个单词  yy复制一行
        * u 撤销  ctrl+r 反撤销
 
