# 「游趣体」变体序列一览表 
## Unicode 标准化变体序列  
Unicode 标准化变体序列 (Standardized Variation Sequences, SVS) 资料来源：https://www.unicode.org/Public/16.0.0/ucd/StandardizedVariants.txt

根据 Unicode 16.0 相关文档，0.300 版本新增 Unicode 变体序列（UVS）支持，在允许使用 UVS 的情况下，可通过该功能实现标点符号的切换。  
支持的标准化变体序列如下表：  
| 字符 | Unicode | + `U+FE00` | + `U+FE01` | 
| :-------: | :-------: | :--------: | :--------: | 
| 0 | `U+30` | 斜线零[0︀] |
| ０ | `U+FF10` | 斜线零[0︀] |
| ， | `U+FF0C` | 左下[<span lang="zh-cn">，︀</span>] | 居中[<span lang="zh-tw">，︁</span>] |
| ． | `U+FF0E` | 左下[<span lang="zh-cn">．︀</span>] | 居中[<span lang="zh-tw">．︁</span>] |
| 、 | `U+3001` | 左下[<span lang="zh-cn">、︀</span>] | 居中[<span lang="zh-tw">、︁</span>] |
| 。 | `U+3002` | 左下[<span lang="zh-cn">。︀</span>] | 居中[<span lang="zh-tw">。︁</span>] |
| ： | `U+FF1A` | 左下[<span lang="zh-cn">：︀</span>] | 居中[<span lang="zh-tw">：︁</span>] |
| ； | `U+FF1B` | 左下[<span lang="zh-cn">；︀</span>] | 居中[<span lang="zh-tw">；︁</span>] |
| ！ | `U+FF01` | 居左[<span lang="zh-cn">！︀</span>] | 居中[<span lang="zh-tw">！︁</span>] |
| ？ | `U+FF1F` | 居左[<span lang="zh-cn">？︀</span>] | 居中[<span lang="zh-tw">？︁</span>] |
| “ | `U+201C` | 非全宽[“] | 全宽[“︁] |
| ” | `U+201D` | 非全宽[”] | 全宽[”︁] |
| ‘ | `U+2018` | 非全宽[‘] | 全宽[‘︁] |
| ’ | `U+2019` | 非全宽[’] | 全宽[’︁] |

> [!NOTE]
> 1. 若全角标点在横排时偏置（靠左下方），则竖排时靠右上方偏置。反之若标点横排时置中，则竖排位置不变。  
> 2. 此规定可能与 UAX#50 规则冲突，部分软件可能因此显示异常，具体表现为全角冒号「：」与全角分号「；」直排时翻转 90 度。

## 关于 SVS 的常见问题  
### Q：如何使用全宽弯引号特性？  
A：在 Word (Microsoft 365) 中，在支持变体序列的字符后（如弯引号`“‘’”`）后输入变体选择符的 Unicode 码位（如`FE01`），再按 Alt + X，即可使用变体序列。

### Q：为什么此字体在一些情况下不支持 SVS 特性？ 
A：部分软件不支持此特性，如**WPS Office、PowerPoint (Microsoft 365)** 等，使用时需留意。
