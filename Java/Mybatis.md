## Mybatis 相关知识

### mapper 关键词
**比较符号**：在Mybatis 的 xml 配置文件中，在 xml 中'<'和'>'有特殊的含义,因此无法产生我们想要的比较大小的效果,因此我们需要使用比较的转义字符,主要有两种方式

1. 使用转义字符  
    * **大于 '>'**: `&gt;`
    * **小于 '<'**: `&lt;`
    * **小于等于 '<='**: `&lt;=`
    * **大于等于 '<'**: `&gt;=`

2. 使用 **'<![CDATA[ ]]>'** 标记  
    该标记避免Sql中与xml规范相冲突的字符对xml映射文件的合法性造成影响,使得 **'<![CDATA[ xxx ]]>'**  的 xxx 这部分内容不使用 xml 语法解析


    