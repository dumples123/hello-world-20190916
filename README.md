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
removeClass(" ") 删除样式
.css(" ")  添加样式
jQuery有一个.prop()的方法让你来调整元素的属性.

我们是这样来让按钮不可选的:

$("button").prop("disabled", true);

jQuery的.html()方法可以添加HTML标签和文字到元素，而元素之前的内容都会被方法的内容所替换掉。

我们是通过em[emphasize]标签来重写和强调标题文本的：

$("h3").html("<em>jQuery Playground</em>");

jQuery 还有一个类似的方法叫.text()，它只能改变文本但不能修改标记。换句话说，这个方法只会把传进来的任何东西(包括标记)当成文本来显示。

Query 有一个.remove() 的方法可以移除HTML元素

试着使用.remove()方法来移除页面上的target4元素吧.移除整个元素标签
  
  现在让我们尝试把元素从一个div里移到另外一个div里。

jQuery有一个appendTo()方法可以把选中的元素加到其他元素中。:像剪切一样。

每个HTML元素根据继承属性都有父parent元素。

你可以给目标元素的第三个子元素添加bounce class。

$(".target:nth-child(3)").addClass("animated bounce");

示例：获取class为target且索引为奇数的所有元素，并给他们添加class。

$(".target:odd").addClass("animated shake");

记住，jQuery里的索引是从0开始的，也就是说：:odd 选择第2、4、6个元素，因为target#2(索引为1)，target#4(索引为3)，target6(索引为5
even:所有偶数
odd:所有奇数

#JavaScript提供七种不同的data types(数据类型)，它们是undefined（未定义）, null（空）, boolean（布尔型）, string（字符串）, symbol(符号), number（数字）, and object（对象）。
  

 使用 ++ ，我们可以很容易地对变量进行自增或者+1运算。

i++;

等效于

i = i + 1;

#.length ,字符串
[]叫中括号，{}叫大括号，()叫小括号。
使用 数组，我们可以在一个地方存储多个数据。

你以左方括号[开始定义一个数组，以右方括号]结束定义，并把每个条目之间用逗号隔开，就像这样：
var sandwich = ["peanut butter", "jelly", "bread"]。
与字符串的数据不可变不同，数组的数据是可变的，并且可以自由地改变。

例如

var ourArray = [3,2,1];
ourArray[0] = 1; // ourArray等于 [1,2,1]


一个简单的方法将数据追加到一个数组的末尾是通过 push() 函数。

.push() 接受把一个或多个参数，并把它“推”入到数组的末尾。

var arr = [1,2,3];
arr.push(4);
// 现在arr的值为 [1,2,3,4]

改变数组中数据的另一种方法是用 .pop() 函数。

.pop() 函数用来“抛出”一个数组末尾的值。我们可以把这个“抛出”的值赋给一个变量存储起来。

这就是 .shift() 的用武之地。它的工作原理就像 .pop()，但它移除的是第一个元素，而不是最后一个，返回第一个元素

.push() 接受把一个或多个参数，并把它“推”入到数组的末尾。

.unshift() 函数用起来就像 .push() 函数一样, 但不是在数组的末尾添加元素，而是在数组的头部添加元素。
function myTest(val) {
  var answer = "";
  // 请把你的代码写在这条注释以下
  switch(val){
    case 1:
     answer="alpha";
      break;
     case 2:
        answer="beta";
      break;
      case 3:
         answer="gamma";
      break;      
      case  4:
        answer="delta";
      break;
      
  }
  
  
  // 请把你的代码写在这条注释以上
  return answer;  
}

// 你可以修改这一行来测试你的代码
myTest(1);




   
  






