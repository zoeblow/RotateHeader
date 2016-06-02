# RotateHeader
RotateHeader 是一款PC端的头像旋转插件，可以随着鼠标的移动切换不同图片，从而达到不同的效果效果。
-----
### 效果
![RotateHeader-preview](https://raw.githubusercontent.com/zoeblow/RotateHeader/master/RotateHeader.gif)


### 创建时间 2016-6-2 17:03:00
#### 作者 [@zoeblow](http://fuyuan.me)
###版本
 ------

> * V 1.0
> * 修改时间 ：2016-6-2 17:03:00
> * 描述：新建RotateHeader github库
    
-----
###调用方式
在html中引入jquery之后引入RotateHeader.js
完成之后即可直接使用
```JavaScript
    // 鼠标位置
    var mouseX;
    var mouseY;
    var imageOne;
    //初始化
    $(init);
    $(window).load(init);
    $(window).resize(init);
    //鼠标移动
    $(window).mousemove(getMousePosition);
    //初始化函数
    function init() {
        mouseX = 0;
        mouseY = 0;
        imageOne = new RotateHeader("one");
    }
    //实时获取鼠标位置
    function getMousePosition(event) {
        mouseX = event.pageX;
        mouseY = event.pageY;
        imageOne.setImageDirection();
    }
```
-----
###参数
| 参数    | 取值类型   |  默认值  | 描述|
| :----:  | :----:  | :----:  | :----:  |
| className    | String |   空     | 旋转的元素 |

