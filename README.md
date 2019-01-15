﻿# CapsX

## 入门教程第一
首先，你需要安装了 [AutoHotKey](https://autohotkey.com/)。
推荐使用的版本： `AutoHotKey_L Unicode x32` （鼠标模拟功能不支持64位）

然后双击 `CapsX.ahk` 来启动 CapsX

> 某些功能需要使用管理员身份运行
> 
> 在 CapsX-Settings.ahk 中
> 
> 手动修改 global T_AskRunAsAdmin := 1 即可



## 使用手册第二

按 `CapsLock` 切换 CapsX 模式
按住 `CapsLock` 使用临时 CapsX 模式

### 按键表
每个模块可以单独禁用，请见 `CapsX-Settings.ahk` 文件

<!-- 下面这堆东西是自动从各个模块里抽取的，如需改动请到模块里操作 -->
<!-- 开始：抽取模块帮助 -->
<!-- 模块帮助文件名：01-插件-模拟鼠标.ahk-->
#### 模拟鼠标模块
| 模式 | 模拟鼠标模块 | 说明 |
| - | :-: | - |
| CapsX | w a s d   | 鼠标平滑移动 |
| CapsX | r f       | 垂直平滑滚轮（在chrome下有时失灵，原因未明) |
| CapsX | R F       | 水平平滑滚轮（在chrome下有时失灵，原因未明) |
| CapsX | rf        | r f一起按相当于鼠标中键 |
| CapsX | e         | 鼠标左键 |
| CapsX | q         | 鼠标右键 |

<!-- 模块帮助文件名：03-应用-Anki增强.ahk-->
#### Anki增强模块
| 模式 | Anki增强模块   | 说明 |
| - | :-: | - |
| 在Anki内 | w 或 k 或 ↑ | 撤销 / 松开显示答案 |
| 在Anki内 | a 或 h 或 ← | 顺利 / 松开显示答案 |
| 在Anki内 | s 或 j 或 ↓ | 困难 / 松开显示答案 |
| 在Anki内 | d 或 l 或 → | 生疏 / 松开显示答案 |
| 在Anki内 | q | 返回上个界面 |
| 在Anki内 | c | 添加新卡片 |
| 在Anki内 | 5 或 Num5 | 撤销 |
| 在Anki内 | 6 或 Num6 | 暂停卡片 |
| 在Anki内 | Alt + I | 快速导入剪贴版的内容 |

<!-- 模块帮助文件名：功能-秒打时间戳.ahk-->
#### 秒打时间戳模块
| 模式 | 秒打时间戳   | 说明 |
| - | :-: | - |
| 全局 | [d 或 (d | 插入日期, 类似 [20190115] 这样的时间戳 |
| 全局 | [t 或 (t | 插入时间, 类似 [20190115.164744] 这样的时间戳 |
| 全局 | [s 或 (s | 插入时间, 类似 [1647] 这样的时间戳 |
| 全局 | [v | 插入版本号, 类似 v2019.01.15 这样的版本号 |

<!-- 模块帮助文件名：应用-Edge增强.ahk-->
#### Edge增强模块
| 模式 | 按键  | 说明 |
| - | :-: | - |
| 在Edge内 | Alt + w | 拿出笔（全屏模式暂时不支持）|
| 在Edge内 | Alt + q | 换左边的笔/橡皮（全屏模式暂时不支持） |
| 在Edge内 | Alt + e | 换右边的笔/橡皮（全屏模式暂时不支持） |
| 在Edge内 | Alt + , | 上一章/节 |
| 在Edge内 | Alt + . | 下一章/节 |
| 在Edge内 | Alt + / | 显示目录 |
| 在Edge内 | Alt + ; | 切换自适应页面大小模式 |
| 在Edge内 | Alt + ' | 切换双页布局模式 |

<!-- 模块帮助文件名：应用-mstsc远程桌面增强.ahk-->
#### mstsc远程桌面增强模块
| 功能 | 说明 |
| - | :-: | - |
| 自动 | 自动置底：如果当前操作的远程桌面窗口是最大化的窗口，则自动置底，这样可以跟当前电脑桌面上的窗口共同操作 |
| RAlt + RCtrl| 切换焦点：右边的 Alt+Ctrl 一起按可以切换焦点在不在远程桌面窗口 |

<!-- 模块帮助文件名：应用-TIM添加常驻功能.ahk-->
#### TIM添加常驻功能模块
|模式|按键|功能|
| - | :-: | - |
| 在Tim窗口内 |Alt + f| 焦点定位到左上角搜索框|
| 在Tim窗口内 |Ctrl + PgUp| 切换上一个窗口|
| 在Tim窗口内 |Ctrl + PgDn| 切换下一个窗口|

<!-- 模块帮助文件名：插件-02-窗口增强.ahk-->
#### 窗口增强模块
| 模式 | 窗口增强模块   | 说明 |
| - | :-: | - |
| 全局 | CapsX键 + \ | 打开多桌面视图 |
| 全局 | CapsX键 + [ | 切换到上一个桌面 |
| 全局 | CapsX键 + ] | 切换到下一个桌面 |
| 全局 | CapsX键 + Alt + [ | 把当前窗口移到上一个桌面 |
| 全局 | CapsX键 + Alt + ] | 把当前窗口移到下一个桌面 |
| 全局 | CapsX键 + = | 新建桌面 |
| 全局 | CapsX键 + - | 合并当前桌面 |
| 全局 | CapsX键 + 0 | 新建桌面，并把当前窗口移过去 |
| 全局 | CapsX键 + 1 | 把当前窗口移到第1个桌面(如果有的话) |
| 全局 | CapsX键 + 2 | 把当前窗口移到第2个桌面(如果有的话) |
| 全局 | CapsX键 + 3 | 把当前窗口移到第3个桌面(如果有的话) |
| 全局 | CapsX键 + 4 | 把当前窗口移到第4个桌面(如果有的话) |
| 全局 | CapsX键 + 5 | 把当前窗口移到第5个桌面(如果有的话) |
| 全局 | CapsX键 + 6 | 把当前窗口移到第6个桌面(如果有的话) |
| 全局 | CapsX键 + 7 | 把当前窗口移到第7个桌面(如果有的话) |
| 全局 | CapsX键 + 8 | 把当前窗口移到第8个桌面(如果有的话) |
| 全局 | CapsX键 + 9 | 把当前窗口移到第9个桌面(如果有的话) |
| Alt+Tab界面下 | w a s d | 切换窗口选择 |
| 窗口靠边界面下 | w a s d | 切换窗口选择 |
| 窗口靠边界面下 | x | 关掉选择的窗口 |
| Win+Tab界面下 | w a s d | 切换窗口选择 |
| Win+Tab界面下 | q e | 左右切换桌面概览
| Win+Tab界面下 | z | 合并当前桌面与上一个桌面
| Win+Tab界面下 | x | 关掉选择的窗口
| Win+Tab界面下 | 1 2 3 ... 9 0 | 把窗口移到除了自己的第x个桌面（或新建桌面） |
| Win+Tab界面下 | v | 新建桌面，并把当前窗口扔到新建桌面 |
| Win+Tab界面下 | c | 新建桌面，并把当前窗口扔到新建桌面，并激活窗口 |
| Win+Tab界面下 | \ | 相当于按下 Tab |
| Win+Tab界面下 | [ | 切换到上一个桌面 |
| Win+Tab界面下 | ] | 切换到下一个桌面 |

<!-- 模块帮助文件名：插件-媒体键.ahk-->
#### 媒体键模块
| 模式 | 媒体键模块   | 说明 （这个模块基本还是半成品。。欢迎push） |
| - | :-: | - |
| CapsX | F5   | 暂停播放 |
| CapsX | F6   | 上一首 |
| CapsX | F7   | 下一首 |
| CapsX | F8   | 停止播放 |
| CapsX | F10  | 静音 |
| CapsX | F11  | 音量减 |
| CapsX | F12  | 音量加 |

<!-- 模块帮助文件名：插件-搜索键.ahk-->
#### 搜索键模块
| 模式 | 搜索键模块   | 说明 （这个模块基本还是半成品。。欢迎push） |
| - | :-: | - |
| CapsX | g    | 用 google 搜索当前选择或鼠标所指的词 |

<!-- 模块帮助文件名：插件-编辑增强.ahk-->
#### 编辑增强模块
| 模式 | Edit模块   | 说明 （这个模块基本还是半成品。。欢迎来改）|
| - | :-: | - |
| CapsX | h l       | 左右方向键 |
| CapsX | k j       | 上下方向键 |
| CapsX | hl        | h l 一起按选择光标下的单词词 |
| CapsX | nm        | n m 一起按选择当前行 |
| CapsX | b         | BackSpace |
| CapsX | B         | Delete |
| CapsX | u         | 撤销 |
| CapsX | U         | 重做 |

<!-- 模块帮助文件名：插件-雪星转屏.ahk-->
#### 雪星转屏模块
| 模式 | 按键 | 功能 |
| - | :-: | - |
| CapsX + | 方向键 上 下 左 右 | 同时旋转所有屏幕到你指定的方向 |
<!-- 结束：抽取模块帮助 -->

## 发展路线第三

简化电脑操作逻辑，提升效率，尽量不与习惯键位冲突

po主偷懒中:
1. [ ] 长按CapsX键显示对应帮助
2. 

## 制作背景第四

本人比较经常写代码……

起初我是右鼠……后来觉得鼠标放右边有点远……改成了左鼠

左鼠之后发现手还是要离开键盘……于是做了这个

## 相关答疑第五
本人常驻 QQ群：271105729

关于这个脚本，相关答疑直接进群提问即可