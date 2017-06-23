这里有更多的资料哈（shang.qq.com/wpa/qunwpa?idkey=4310b023aa9a592a667889be958934a341cf5d062ed93a41402a5fddc9056281）验证码022

# 运行效果

![](http://i.imgur.com/TPkIrBJ.gif)



## 使用步骤

### 1. 在project的build.gradle添加如下代码(如下图)

	allprojects {
	    repositories {
	        ...
	        maven { url "https://jitpack.io" }
	    }
	}

![](http://oi5nqn6ce.bkt.clouddn.com/itheima/booster/code/jitpack.png)


### 2. 在Module的build.gradle添加依赖

     compile 'com.github.open-android:WheelPicker:v1.0.0'


### 3. 复制如下代码到xml

    <com.itheima.wheelpicker.WheelPicker
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:wheel_atmospheric="true"
        app:wheel_curved="true"
        app:wheel_cyclic="true"
        app:wheel_selected_item_position="5"
        app:wheel_item_text_color="#66ff0000"
		app:wheel_selected_item_text_color="#6600ffff"/>


    <!--属性解释:
	
        wheel_atmospheric :  条目颜色是否执行衔接处理 效果更好
        wheel_curved ： 是否是弧形状态显示
        wheel_cyclic : 是否可循环
        wheel_selected_item_position ： 默认选中第几个条目
        wheel_item_text_color 未选中的条目颜色
        wheel_selected_item_text_color  选中的条目颜色-->

###4 . 运行即可

#### 细节注意:

> 默认会自带一组数据，所以无需设置数据。 若想设置新的数据，可通过 调用如下方法即可

		setData(List data); 

* 详细的使用方法在DEMO里面都演示啦,如果你觉得这个库还不错,请赏我一颗star吧~~~

* 欢迎关注微信公众号

![](http://mmbiz.qpic.cn/mmbiz_jpg/SGLMEl6egy86amMN9XlltwZamViaKibz8J4aVZB5XqU1SwIhLHe3ZMiaTv4tMmNo0YUqJbZbrjfsQemWnp0LpeSpg/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1)
