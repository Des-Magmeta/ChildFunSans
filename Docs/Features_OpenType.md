<!--
# `calt` 上下文替代字
生效规则：默认宽度（比例）和等宽（半宽）宽度下，「数字+英文冒号（`:`）+数字」组合出现时，冒号自动居中。
> 例：输入`12:34`  
> 上下文替代字启用前：`one two` `colon` `three four`  
> 上下文替代字启用后：`one two` `colon.calt`**`three four`
-->

# 漫画排版使用连字
该领域涉及特性：
- `dlig` Discretionary Ligatures | 自由连字 | 自選連字
- `vert` Vertical forms | 竖直书写形式 | 縱書形式
- `cpct`/`ss01` Centered CJK Punctuation | 全角标点居中 | 全形置中標點
- `ss03` Titled Punctuation | 漫画标点符号 | 漫畫標點符號
- `ss04` Third width | 三分宽数字与符号 | 三分之一寬度字
- `ss05` Quarter width | 四分宽数字与符号 | 四分之一寬度字

支持自由连字(`dlig`)的字符组合及其倾斜标点(`ss03`)可用情况见下表：
**`ss03`是否支持** | **描述** | **Unicode** | **字符(仅限已入Ｕ)** | **字符组合** 
 --- | --- | --- | --- | --- 
　| 双重问号 | U+2047 |⁇| ？？ 
　| 三重问号 | U+FF1F U+FF1F U+FF1F | | ？？？
Y | 双重叹号 | U+203C |‼| ！！
Y | 三重叹号 | U+FF01 U+FF01 U+FF01 | | ！！！
Y | 四重叹号 | U+FF01 U+FF01 U+FF01 U+FF01 | | ！！！！
Y | 五重叹号 | U+FF01 U+FF01 U+FF01 U+FF01 U+FF01 | | ！！！！！ 
Y | 问叹号 | U+2048 |⁈| ？！
Y | 叹问号 | U+2049 |⁉| ！？ 
　| 双重问号与叹号 | U+FF1F U+FF1F U+FF01 | | ？？！
　| 问-叹-问号 | U+FF1F U+FF01 U+FF1F | | ？！？
　| 叹号与双重问号 | U+FF01 U+FF1F U+FF1F | | ！？？
　| 双重叹号与问号 | U+FF01 U+FF01 U+FF1F| | ！！？
　| 叹-问-叹号 | U+FF01 U+FF1F U+FF01 | | ！？！
　| 问号与双重叹号 | U+FF1F U+FF01 U+FF01 | | ？！！
　| 双重叹号与双重问号 | U+FF01 U+FF01 U+FF1F U+FF1F| | ！！？？
　| 双重问号与双重叹号 | U+FF1F U+FF1F U+FF01 U+FF01| | ？？！！

 ①上表中，「Y」标记为是；  
 ②将`U+FF01`替换为`U+FE15`、`U+FF1F`替换为`U+FE16`（等价于竖排情况）时此特性同样生效。
