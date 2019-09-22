# hello-world-20190916
学习第一天，为了抓取时间自由,20190916/10/40
前端笔记：
CSS:
这个为内联样式
<h2 style="color: red">CatPhotoApp</h2>，你就给h2元素添加了inline style(内联样式)
但是更易于维护的方式是使用层叠样式表CSS（Cascading Style Sheets）。
1.元素选择器
f:<style>
  选择器 {属性名称: 属性值;}
  h2 {color: red;}
</style>
2.类选择器
3.id 选择器

1.布局

2元素样式优先级别
  类：color: pink !important>内联样式> id选择器>类选择器下面的优先级>类上面的优先级
  
  
#响应式框架Bootstrap
Bootstrap 使用一种响应式网格布局
<link href="//fonts.gdgdocs.org/css?family=Lobster" rel="stylesheet" type="text/css">
<link rel="stylesheet" href="//cdn.bootcss.com/bootstrap/3.3.1/css/bootstrap.min.css"/>

然后直接引用其中的class 来调试页面
<div > class ="container-fluid"  </div> :  <div> 里面的自动排版
class="img-responsive”  : 图片自动适应屏幕大小；
class ="text-center"  图片居中
class ="btn"  button 按钮样式
class ="btn-block" button 属性 ，自动填充按钮至水平，下一块自动换行
calss ="btn-primary "  自动添加颜色：深蓝色
class= "btn-info"  浅蓝色
 #图库
  Font Awesome  ：图标库 这些图片都是矢量图，以 .svg 文件格式保存
<link rel="stylesheet" href="//cdn.bootcss.com/font-awesome/4.2.0/css/font-awesome.min.css"/>
<i class="fa fa-info-circle"></i> : 指代图标
  
 <button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info"><i class ="fa fa-info-circle"></i> info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger"><i class ="fa fa-trash"></i> Delete</button>
    </div>
  点赞图标，信息图标，删除图标
 #Jquery 选择器
现在你已经了解了3种选择器：
元素选择器：$("button")、
class选择器：$(".btn")、
id选择器：$("#target1")。

  
  

 
   
  






