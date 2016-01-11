#### 简单的链接样式
> 链接分为：内部链接，外部链接

* 外部链接伪类：
    * :link 没有访问过的链接
    * :visited 被访问的链接
    
* 全部元素动态伪类：
    * :hover 鼠标悬停元素
    * :active 鼠标点击瞬间
    * :focus 键盘焦点
> ps: 由于层叠原因，需要使用这种顺序保证链接不会失效：link;visited;hover;focus;active;(lord vader hates furry animals)

#### 关于[全部]下划线
> 下划线的作用是用来对于视觉障碍的人区分的

* 未完成访问的下划线样式（静止，浮动，点击）
    * 简单下划线方案
        1. 默认：去掉下划线，将链接加粗 | 悬浮或激活：重新应用下划线
        1. 默认：应用边框做点线 | 悬浮或激活：将边框点线连成实线
    
    * 奇特的链接下划线
    > 通过应用背景创建简单的下划线图像

* 已经访问的下划线样式
> 避免用户不必要的‘回朔’操作
    * 为访问的目标设置样式（跳到目标文本）
       > :target (css3)设置目标元素的样式 IE不支持

#### 突出[部分]链接       
* 突出显示不同类型的链接
>外部链接添加(图标)
    * 手动添加类
    >.external{background:url();pading-right:10px;}
    * 自动添加类(css3)
    >[attr = ^val] :属性选择器，前部选择
    
* 突出可下载的文档和提示
    > [attr = $val]: 属性选择器，尾部选择

#### 创建类似于按钮的链接
> 将display属性设置为block PS:post请求需要实用表单元素，这个只能用于get请求，不能用于post请求
    宽度：em
    高度：line-height

* 颜色的反转
    > ：hover属性设置进行反转
* 图像的反转
    > ：hover属性设置进行反转
* CSS精灵
    > 将所有图标放在一个图片中，通过设置background-position来设置位置
* CSS3实现反转
    > text-shadow,box-shadow,border-radius,gradient(渐变),box-reflect(倒影)

#### 纯css工具提示
    绝对定位元素定位最近已经定位的祖先元素(一般一个是relative，一个是absolute)
    
    
    

        