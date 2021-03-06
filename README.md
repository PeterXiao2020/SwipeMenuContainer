# SwipeMenuContainer
[![](https://www.jitpack.io/v/qdxxxx/SwipeMenuContainer.svg)](https://www.jitpack.io/#qdxxxx/SwipeMenuContainer)
[![](https://badge.juejin.im/entry/59a97b39f265da24722fe004/likes.svg?style=flat)](https://juejin.im/user/57028e8f2e958a0059237a6b)
<br/>
仿QQ向左滑动弹出菜单的布局.

 ![image](https://github.com/qdxxxx/SwipeMenuContainer/blob/master/appGif/demo.gif)
 
  ---
 ### Download
 [https://fir.im/6q2m]( https://fir.im/6q2m)
 
  ---
### 集成方式

 - 注入依赖
 Step 1. Add the JitPack repository to your build file
 Step 2. Add the dependency
```
	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
```
	dependencies {
 	   compile 'com.github.qdxxxx:SwipeMenuContainer:v1.0.3'
	}
```

#### Layout
```
    <qdx.swipemenucontainer.SwipeMenuLayout
        android:layout_width="match_parent"
        android:layout_height="70dp"
        qdx:isLeftMenu="false"     //false(右侧是菜单),true(左侧是菜单)    
       ...
        />
```
<br/>

### 兼容超强的[BaseRecyclerViewAdapterHelper]( https://github.com/CymChad/BaseRecyclerViewAdapterHelper)
---

#### 普通RecyclerView item.
 ![image](https://github.com/qdxxxx/SwipeMenuContainer/blob/master/appGif/normal.gif)
 
 <br/>
 
#### 多种itemType
![image](https://github.com/qdxxxx/SwipeMenuContainer/blob/master/appGif/mulit.gif)
<br/>
  
#### 长按拖拽
需要设置```enableParentLongClick(tren)```允许父类拖拽.

![image](https://github.com/qdxxxx/SwipeMenuContainer/blob/master/appGif/drag.gif)
<br/>
   
#### 多级item
![image](https://github.com/qdxxxx/SwipeMenuContainer/blob/master/appGif/expandable.gif)
 <br/>
 

### 方法及属性介绍
---

name                   | format                  |中文解释
----                   |------                   |----
isLeftMenu             | boolean  		 |菜单是否在内容左边（如果在左边，则右滑）
enableParentLongClick  | boolean    		 |允许父类长按（此时内容就会被拦截down事件）                     
expandRatio            | float   		 |菜单能够自动打开的阈值
expandDuration 	       | integer     		 |菜单展开动画时间
collapseRatio          | float	      	         |菜单能够自动关闭的阈值
collapseDuration       | integer 		 |菜单关闭动画时间
collapseInstant	       | void                    |不显示动画,关闭菜单
collapseSmooth	       | void                    |平滑关闭菜单
expandSmooth	       | void                    |平滑打开菜单
<br/>


### THANKS
---
  借鉴[SwipeDelMenuLayout]( https://github.com/mcxtzhang/SwipeDelMenuLayout)
  
  超强的[BaseRecyclerViewAdapterHelper]( https://github.com/CymChad/BaseRecyclerViewAdapterHelper)


<br/>

### Artical
---

博客详解文章[http://blog.csdn.net/qian520ao/article/details/77587904](http://blog.csdn.net/qian520ao/article/details/77587904)



###  License
---

```
MIT License

Copyright (c) 2017 qdx

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```



