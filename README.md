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

  input type="text" id="searchStartTime" class="Wdate" onclick="showdate1()"

  class="Wdate" 为必填项，具体操作看mydate97操作文档，这里做了一个组件库集成

  function showdate1(){
       WdatePicker({dateFmt:'yyyy-MM-dd HH:mm:ss'});
    }

  * 图形界面

![日历](https://github.com/coolfxl/cool-module/blob/master/pictures/date.jpg)

* 树形菜单

  div id="permissiontree" <br/>
  $("#permissiontree").tmTree({})<br/>
  
  var permissions = {"root":[{"name":"所有","opid":1,"pid":1,"url":"javascript:void(0);"},{"name":"审核","opid":10,"pid":10,"url":"javascript:void(0);"},{"name":"查看","opid":11,"pid":11,"url":"javascript:void(0);"},{"name":"工具","opid":12,"pid":12,"url":"javascript:void(0);"},{"name":"模板管理","opid":13,"pid":13,"url":"javascript:void(0);"}],"children":{"1":[{"name":"禁用","opid":2,"pid":2,"url":"javascript:void(0);"},{"name":"搜索","opid":5,"pid":5,"url":"javascript:void(0);"},{"name":"添加","opid":6,"pid":6,"url":"javascript:void(0);"},{"name":"置顶","opid":7,"pid":7,"url":"javascript:void(0);"},{"name":"评论","opid":8,"pid":8,"url":"javascript:void(0);"},{"name":"下单","opid":9,"pid":9,"url":"javascript:void(0);"}],"2":[{"name":"yy7y","opid":20,"pid":20,"url":"javascript:void(0);"}]}}

  
  $("#permissiontree").tmTree({
  
      rightMenu:true,root:root,children:children,type:"checkbox",callback:function($opTarget, params, model){
        
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

  * 图形界面
![树形菜单](https://github.com/coolfxl/cool-module/blob/master/pictures/more-tree.png)

