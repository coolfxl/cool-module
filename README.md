# cool-module
js组件库，最终版，附带操作说明

#具体操作
引进资源文件

<!-- 分页样式 -->

<link rel="stylesheet" type="text/css" href="css/css/tz-page.css"/>

<!-- js组件库所有的样式 -->

<link rel="stylesheet" href="css/css/sg.css" />

<!-- 树形菜单样式 -->

<link rel="stylesheet" type="text/css" href="tree/tm_tree.css"/>

<!-- 引入jQuery依赖 -->

<script type="text/javascript" src="js/jquery-1.11.2.min.js"></script>

<!-- 树形菜单js -->

<script type="text/javascript" src="tree/tm_tree.js" ></script>
<!-- js组件库工具类 -->
<script type="text/javascript" src="js/sgutil.js"></script>
<!-- 组件库js -->
<script type="text/javascript" src="js/sg.js"></script>
<!-- 分页js -->
<script type="text/javascript" src="js/tz_page.js" ></script>
<!-- 日期js -->
<script type="text/javascript" src="js/date/WdatePicker.js" ></script>

#日期

<input type="text" id="searchStartTime" class="Wdate" onclick="showdate1()">
class="Wdate" 为必填项，具体操作看mydate97操作文档，这里做了一个组件库集成
function showdate1(){
   WdatePicker({dateFmt:'yyyy-MM-dd HH:mm:ss'});
}
图形界面
![日历](https://github.com/coolfxl/cool-module/blob/master/pictures/date.jpg)

![]()

