# `calt` 上下文替代字
生效规则：默认宽度（比例）和等宽（半宽）宽度下，「数字+英文冒号（`:`）+数字」组合出现时，冒号自动居中。
> 例：输入`12:34`  
> 上下文替代字启用前：`one two` `colon` `three four`  
> 上下文替代字启用后：`one two` `colon.calt`**`three four`


# 漫画排版使用连字
该领域涉及特性：
- `dlig` Discretionary Ligatures | 自由连字 | 自選連字
- `vert` Vertical forms | 竖直书写形式 | 縱書形式
- `cpct`/`ss01` Centered CJK Punctuation | 全角标点居中 | 全形置中標點
- `ss03` Titled Punctuation | 漫画标点符号 | 漫畫標點符號
- `ss04` Third width | 三分宽数字与符号 | 三分之一寬度字
- `ss05` Quarter width | 四分宽数字与符号 | 四分之一寬度字
  
**`ss03`是否支持** | **描述** | **Unicode** | **字符(仅限已入Ｕ)** | **字符组合** 
 --- | --- | --- | --- | --- 
　| DOUBLE QUESTION MARK | U+2047 |⁇| ？？ 
　| TRIPLE QUESTION MARK | U+FF1F U+FF1F U+FF1F | | ？？？
Y | DOUBLE EXCLAMATION | U+203C |‼| ！！
Y | TRIPLE EXCLAMATION | U+FF01 U+FF01 U+FF01 | | ！！！
Y | QUADRUPLE EXCLAMATION | U+FF01 U+FF01 U+FF01 U+FF01 | | ！！！！
Y | QUINTUPLE EXCLAMATION | U+FF01 U+FF01 U+FF01 U+FF01 U+FF01 | | ！！！！！ 
Y | QUESTION EXCLAMATION | U+2048 |⁈| ？！
Y | EXCLAMATION QUESTION | U+2049 |⁉| ！？ 
　| DOUBLE QUESTION EXCLAMATION | U+FF1F U+FF1F U+FF01 | | ？？！
　| QUESTION EXCLAMATION QUESTION | U+FF1F U+FF01 U+FF1F | | ？！？
　| EXCLAMATION DOUBLE QUESTION | U+FF01 U+FF1F U+FF1F | | ！？？
　| DOUBLE EXCLAMATION QUESTION | U+FF01 U+FF01 U+FF1F| | ！！？
　| EXCLAMATION QUESTION EXCLAMATION | U+FF01 U+FF1F U+FF01 | | ！？！
　| QUESTION DOUBLE EXCLAMATION | U+FF1F U+FF01 U+FF01 | | ？！！
　| DOUBLE EXCLAMATION DOUBLE QUESTION | U+FF01 U+FF01 U+FF1F U+FF1F| | ！！？？
　| DOUBLE QUESTION DOUBLE EXCLAMATION | U+FF1F U+FF1F U+FF01 U+FF01| | ？？！！

 上表中，「Y」标记为是。
