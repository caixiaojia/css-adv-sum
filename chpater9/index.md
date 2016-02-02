#### 如何跟踪CSSbug
   * 通用问题
    * 特殊性和层叠行
    * 外边句叠加问题
   * 捕捉bug的基本知识
    1. 检查语法错误
    1. 检查浏览器混杂模式
   * 尽量在开始时候避免bug
    * 查看元素轮廓
    * 如果两个浮动框外边句增大,那么可能是遇到IE的双外边距浮动bug(修复方式:将position设置为relative,将display设置为inline)
   * 创建基本测试案例
    * 复制问题文件,删除多余html,然后注释样式表
    * 求助网站:css-discuss.org,webstandardsgroup.org,stakoverflow.com

#### 神秘的haslaoyout属性
   * 拥有布局
    > 负责本身和子元素的尺寸设置和定位的元素叫做拥有布局.只有IE有这个概念,但是拥有布局会导致性能问题
    * 可以使用javascript,haslayout查看一个元素是否拥有布局
        * float
        * display:inline-block
        * width,height,zoom,writing-modetb-rl
        * overflow:hidden,scroll,auto
        * min-width
        * max-width

#### hack和过滤器
    lve
#### 最常见的浏览器bug以及修复方法
    lve
#### 分级浏览器支持
    lve