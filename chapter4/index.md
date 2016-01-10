#### Background
> Atrr: url,position,image,重点在于position的解释

1. background-position:left center
    left:左边，center：中间，左边垂直居中
1. background-position:10px 10px
    相对于元素左上角，上方偏离10px，左边偏离10px
1. background-position:10% 10%
    以背景图片中10%，10%的点为相对点，相对父元素10%，10%的进行偏移（0,50% 做垂直居中）
    
#### 圆角框
>图片设置遵循，由底下到上面，由外边到里面的原则

* [固定宽度的圆角框](https://github.com/caixiaojia/css-adv-sum/blob/master/chapter4/Radius.html)
> 可以垂直扩展，不可以水平扩展,分为单色和非单色

    * 设置好框体宽度，设置背景颜色
    * 设置好顶部图片
    * [设置中间Body颜色]
    * 设置好底部图片
    
* [可变宽度的圆角框](https://github.com/caixiaojia/css-adv-sum/blob/master/chapter4/Radius.html)
> 可以垂直扩展，可以水平扩展，又称之为滑动门技术
    
    * [设置em，宽度](http://www.cnblogs.com/zhangpengshou/archive/2012/08/04/2623061.html)
    * 设置底部左边图片（一般较长，滑动长度取决于图片的长度）
    * 设置底部右边图片
    * 设置顶部左边图片（一般较长，滑动长度）
    * 设置顶部右边图片
    
#### 山顶角
> 制作图片蒙版，设置透明圆角，覆盖地方为白色
  
  * CSS2实现
    >使用类似于上面那种多个div，然后设置背景属性
  * CSS3实现
      * 多个背景 
        >background-image 可以添加多个背景图片，IE目前不支持，但是看到的是直角框
      * border-radius
        >设置边框角的半径
      * border-image
        >利用九分法缩放作为元素的边框

#### 投影
1. 将一个大的投影图像应用于容器div的背景，然后用负的外边距偏移这个图像
1. 同上，但是使用相对位置偏移图像
1. box-shadow(CSS3)进行偏移,垂直和水平偏移，投影宽度和颜色

#### 不透明度
* RGBa:rgba(x,x,x,x),前三个是颜色，最后面那个是不透明度
* PNG透明度：
    >IE6,7不支持透明 ，配置IE6专用css代码可能会让别的css文件失效:
    <!--[if ie 6]--> **** <!--[endif]-->
* CSS视差效果：
    >将图像相对于窗口水平偏移，就会在改变窗口大小的时候发生改变，从而产生移动，百分比越大，移动的速度越快
    
#### 图像替换
> 将原本显示的文本隐藏，替换成图像，这样会有比较多的样式可以选择

* Phark
> 使用 text-indent:-500px; 进行负文本缩进
    