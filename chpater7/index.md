#### 创建有吸引力且可访问的数据表格
   * 表格特有的元素
    1. summary和caption
        > summary是一个属性,用来描述表格的内容;caption是一个标签用来制作表格的标题
    1. thead和tbody和tfoot
        > thead,tbody,tfoot将表格划分为几个逻辑部分.一个表格中,thead和tfoot只能用一次,tbody可以使用多次.
        
        * 行标题和列标题应该使用th而不是td,表格的标题可以设置值为row(行标题)或者col(列标题)的scope属性,rowgroup(标签)或者colgourp(标签)值表示和多行,多列.       
    1. col和colgroup
        > <colgroup><col/></colgroup> 对列使用样式
        
   * 数据表格标记(实例)
   
       <table summary="a calendar table">
        <!-- 表格标题 -->
            <caption>
                <!-- 列组 -->
                <colgroup>
                <!-- 单列 -->
                    <col id="item1">
                    <col id="item2">
                    <col id="item3">
                    <col id="item4">
                    <col id="item5">
                </colgroup>
            </caption>
            <!-- 逻辑头 -->
            <thead>
                <tr>
                    <th scope="col"></th>
                    <th scope="col"></th>
                    <th scope="col"></th>
                    <th scope="col"></th>
                    <th scope="col"></th>
                </tr>
            </thead>
            <!-- 逻辑body -->
            <tbody>
                <tr>
                    <td><a href="#"></a></td>
                    <td><a href="#"></a></td>
                    <td><a href="#"></a></td>
                    <td><a href="#"></a></td>
                    <td><a href="#"></a></td>
                    <td><a href="#"></a></td>
                    <td><a href="#"></a></td>
                </tr>
            </tbody>
            <!-- 逻辑尾部 -->
            <tfoot>
                <tr>
                    <th></th>
                </tr>
            </tfoot>
        </table>
   * 对表格应用CSS样式
    > 单独的盒模型:每个单元格周围有边框,叠加盒模型:单元格共享边框
    * border-collapse:collapse(叠加盒模型)
    * border-collapse:spearate(单独盒模型)
    * border-spacing:控制单元格之间的距离
#### 创建简单和复杂的表单布局
   * 简单表单布局
    * 有用的表单元素
        > fieldset对信息块进行分组,legend就像是fieldset的标题
        
        * 表单标签
            > lable可以添加结构增加表单的可用性和可访问性,屏幕阅读器会将表单元素和标签联系起来.
            1. 隐式:将表单元素嵌套在label元素中
            1. 显式:label的for属性设置为相关联的表单元素的id名称
        * 基本布局
            >将表单全部设置为块级元素(label for),这让相关联的元素出现在另一行上
            
        <filedset>
            <legend>a calender form</legend>
            <div><label for="">name:<input type="text" id="#"></label></div>
            <div><label for="">name:<input type="text" id="#"></label></div>
            <div><label for="">name:<input type="text" id="#"></label></div>
            <div><label for="">name:<input type="text" id="#"></label></div>
        </filedset>
        <filedset>
            <legend>a calender form</legend>
            <div><label for="">name:<input type="text" id="#"></label></div>
            <div><label for="">name:<input type="text" id="#"></label></div>
            <div><label for="">name:<input type="text" id="#"></label></div>
            <div><label for="">name:<input type="text" id="#"></label></div>
        </filedset>
   * 复杂表单布局
#### 对各种表单元素应用样式
   * 布局
       * 将标签做浮动并且设置宽度让表单元素排齐
   * 其他
       * 如果表单跨多行,需要clear:left
#### 提供可访问的表单反馈
   > 隐藏label:将text-indent:-1000em,将label的宽度设置为0,然后单独设置表单控件尺寸,并且使用外边距控制水平间距
   
   * 多列复选框
    创建步骤:
       * 创建两个filedset,然后设置样式,让两个浮动并列
   * 提交按钮
       * 使用button,type=submit来替代input按钮
   * 表单反馈
       * 父元素relative,子元素absolute
   