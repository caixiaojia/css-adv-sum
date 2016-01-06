#### 语义化重要性
> Notice:项目代码稍微变得复杂之后，header,footer等则会让结构分明，方便维护

1. 机器人：搜索引擎识别
1. 开发者：减少选择器标识符的添加


#### ID和类名
> ID和类名是由于标签语义不丰富产生的次优选择器，在Html5全面开火以后标签更加丰富会一定程度上减少
> 使用，这样会使得文件机构更加精简。

1. ID:
    * 特定且唯一的元素
    * 持久性的结构选择：header，footer等（HTML4)
1. 类:
    * 一组相同的元素
1. 命名
    * 内容：用来做什么
    * 分割：- 进行分割
    * 大小：全部小写

    
#### div和span
>div和span请勿过度使用，避免添加过度div会导致后后期难以维护

1. div:对于块级元素进行分组（竖着)
1. span:对于行内元素进行分组(横着)


#### 微格式
>为了突出人，地点，日期等类型的信息，基于vcard
>开发了一组命名约定来表示这些数据


#### DOCTYPE
1. strict：不允许使用老的元素(font.)，而transitional则允许
1. 浏览器相对应是标准模式和混杂模式，会根据DOCTYPE区分


#### 有效性验证
>用来验证代码是否有效,寻找代码中的Bug

* 工具
    * [W3C Markup Validation Service](http://validator.w3.org/)
    * Firefox web develop extensions

    
#### 总结
    ''' html和css之间的联系和影响。html语义化对于css选择器影响;以及标识头对于浏览器对于css解析影响;约定格式对于css的缺陷弥补；如何查找bug'''
