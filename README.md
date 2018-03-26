# cool-module
js组件库，最终版，附带操作说明

## 具体操作

### 资源引进

* 引进css样式文件
   *  #分页样式
      * link rel="stylesheet" type="text/css" href="css/css/tz-page.css"
   *  树形菜单样式 
      * link rel="stylesheet" type="text/css" href="tree/tm_tree.css"
   *  js组件库所有的样式
      * link rel="stylesheet" href="css/css/sg.css"



* 引进js文件
  * 引入jQuery依赖
    * <script type="text/javascript" src="js/jquery-1.11.2.min.js"></script>
  * 树形菜单js
    * <script type="text/javascript" src="tree/tm_tree.js"></script>
  * js组件库工具类
    * <script type="text/javascript" src="js/sgutil.js"></script>
  * js组件库
    * <script type="text/javascript" src="js/sg.js"></script>
  * 分页js
    * <script type="text/javascript" src="js/tz_page.js"></script>
  * 日期
    * <script type="text/javascript" src="js/date/WdatePicker.js"></script>

### 实际操作

* 日期

  <input type="text" id="searchStartTime" class="Wdate" onclick="showdate1()">

  class="Wdate" 为必填项，具体操作看mydate97操作文档，这里做了一个组件库集成

  function showdate1(){
       WdatePicker({dateFmt:'yyyy-MM-dd HH:mm:ss'});
    }

* 图形界面

![日历](https://github.com/coolfxl/cool-module/blob/master/pictures/date.jpg)

* 树形菜单
  <div id="permissiontree"></div>
  $("#permissiontree").tmTree({})
  $("#permissiontree").tmTree({rightMenu:true,root:root,children:children,type:"checkbox",callback:function($opTarget, params, model){
    var opid = params.opid;//选中节点的id
    if(model == "add"){
    }
    if(model == "edit"){
    }
    if(model == "delete"){
    }
    if(model == "cancel"){
    }
  }});


![]()

