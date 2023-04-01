# jquery
学习经历


#### jQuery

- 1 选择器

  | code | 选取 |
  | ------ | :--- |
  | $("*") | 所有元素 |
  |$("#xxx")|id选择器|
  |$(".xxx")|class选择器|
  |$("element")|标签选择器|
  |$("p:first")|第一个p元素|
  |$("p:last")|最后一个p元素|
  |$("p:even")|选取所以的偶数p元素|
  |$("p:odd")|选取所以的奇数p元素|

- 2 事件

  | code       | 事件     |
  | ---------- | -------- |
  | click      | 鼠标点击 |
  | dbclick    | 鼠标双击 |
  | mouseenter | 鼠标进入 |
  | mouseleave | 鼠标离开 |
  | hover      | 鼠标悬停 |
  | keypress   | 键盘点击 |
  | keydown    | 键盘按下 |
  | keyup      | 键盘松开 |

- 3 效果

  | code          | 效果      |
  | ------------- | --------- |
  | hide()        | 隐藏      |
  | show()        | 显示      |
  | toggle()      | 显示/隐藏 |
  |||
  | fadeIn()      | 淡入      |
  | fadeOut()     | 淡出      |
  | fade Toggle() | 淡入/淡出 |
  | fadeTo() | 给定不透明度(0-1) |
  |||
  | slideDown() | 向下滑动 |
  | slideUp() | 向上滑动 |
  | SlideToggle() | 上/下滑动 |
  | slideToggle(slow) | 慢速滑动 |
  | slideToggle(fast) | 快速滑动 |
  | slideToggle(speed()) | speed设置时长 |
  |      |      |
  | animate() | 创建动画 |
  | animate({}) | 动画多个属性 |

- 3 Ajax

  | code      |          |
  | --------- | -------- |
  | load(url) | 加载数据 |
  
  ```javascript
  $("xxx").click(function(){	
      //点击事件
    $("xxx").load("demo_test.txt",function(responseMessage,status,response){
      //三个参数,调用成功时的结果,调用的状态,XMLHttpRequest对象
      if(statusTxt=="success")
          console.log("数据加载成功")
      if(statusTxt=="error")
          console.log("数据加载失败")
        alert("Error: "+resopnse.status+": "+resopnse.status);
    });
  });
  ```
