<!doctype html>
<html>
<head>
<meta charset="UTF-8">
<title>表单demo</title>
</head>

<body>
<form autocomplete="on">
<p> 名字：<input type="text" value="" placeholder="请输入姓名"></p>
<p> 密码：<input type="password"></p>
<p>数字：<input type="number" required></p>
<p>时间：<input type="date"></p>
<p>
性别：男<input type="radio" name="sex" checked  value="male"> 女<input type="radio" name="sex" value="female"> <!--里面要发送对应的值，不是控件中的值-->
</p>
<p>
选择你的爱好：游泳<input type="checkbox"  name="hobby"  value="swimming">足球<input type="checkbox"   name="hobby" value="football">篮球<input type="checkbox"   name="hobby" value="basketball"><!--成组必须写上name值。写上value-->

</p>
<!--使用label属性来扩大点击范围
--><p><label><input type="checkbox">我同意该协议</label></p>
<input type="checkbox" id="favorer">
<p>
  下拉列表：
 <select multiple  size="4"><!--multiple 选择多重的 想要多选 ctrl健多选 szie 可见选项的树木-->
<option > 请选择你所在的省份</option>
<option  selected>河南</option><!--想要出现默认的就在里面加上 selected-->
<option> 河北</option>
<option>山东</option>
<option>青海</option>

<optgroup label="华东地区">
<option>西藏</option>
<option>上海</option>
</optgroup>

<optgroup label="华北地区">北方
<option>南京</option>
<option>湖南</option>
</optgroup>
<!--每一个opt都有一个value的定义-->
 </select>
</p>
选择你喜欢的浏览器：
<input  list="browersselect" >
<datalist id="browersselect">
<option value="IE">IE666</option>
<option value="FIRE" label="火狐">firefox</option>
<option>360</option>
<option>google</option>
<!--1和下拉列表的区别，下拉列表智能选择给的选项，这个提示列表是可以输入列表中没有的内容。2主要现实浏览器的value所以要写上opt的值，google和火狐中显示的不同-->
</datalist>


<h5>通用的事件型按钮</h5>
<p>普通按钮：<input type="button" value="普通按钮"></p>
<p>提交按钮：<input type="submit" value="立即提交"></p><!--每一个表单都有一个提交按钮-->
<p>重置按钮：<input type="reset" value="重置"></p><!--每一个表单都有一个提交按钮-->
<p>图像按钮：<input type="image"  src="timg (2).jpeg" width="100" height="40" ></p>
<p> 文件上传：<input type="file"  multiple></p><!--多选的属性multiple-->
  First name: <input type="text" name="fname" autofocus><br>
  Last name: <input type="text" name="lname"><br>
  <input type="submit">
  <label  for="favorer"><p>我是上面的checkbox</p></label>
</form>
<!--配合脚本实现，传统方式做的：做一个盒子，先把列表项写进去，然后输入的时候显示，不输入的时候消失，一般都是搜索联想输入。-->



</body>
</html>

