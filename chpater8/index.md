## css布局三个基本概念:定位,浮动,外边距操纵
### 创建可伸缩且容易维护的css系统:1.检查设计,2.寻找重复模式.
   * 具体步骤
    1. 划分大的结构区域:页头,页脚
    1. 结构区域的内容区域,开始建立网格机构
    1. 在内容区域设置不同的布局结构,分成几列
    1. 结构设计完之后开始关注内容,然后起名字
    
    1. 然后看是否有公用的模式,尽量采用一般的类名,根据上下文应用样式
    1. 立即确定不同内容类型的细节
#### 让设计在页面中水平居中
    * 使用外边距让设计居中
        * 设置wrapper类
        * margin:0 auto 让水平居中
#### 创建两列和三列基于浮动的布局
    * 基于浮动的布局(2列)
        > 一个向左,一个向右浮动,然后添加display:inline属性防止IE中的双外边距浮动产生的bug
        
        >父元素使用overflow:hidden;防止下方的页脚提升
    * 基于浮动的布局(3列)
        >基于2列浮动的2次嵌套
#### 创建固定宽度,流式和弹性布局
    * 流式布局
        * 将宽度全部设置为百分比
        * 设置最小的min-width,或者max-width,em
    * 弹性布局
        * 将宽度设置为em,而且要设置max-width防止出现滚动条
        * 大多数浏览器默认字号是16px,10像素大概是62.5%,设置字体为62.5%时候,1em大概是10px
    * 流式和弹性图片
        * 将百分比和max-width配合进行设置
    * faux列
        * 设置父元素重复的背景用来达到背景统一的目的 
#### 创建高度相等的列
    * 通用:相当于一个垂直滑动门
    * CSS3 列:column-count(列数),column-width(宽度),column-gap(间距)
#### css框架和css系统
    * bootstrap之类