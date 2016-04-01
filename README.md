##1，工具：


- [图形可视化编程器](http://labs.udacity.com/android-visualizer/#/android/sandbox)
- [设计规范](https://www.google.com/design/spec/material-design/introduction.html)
- [开发文档](https://developer.android.com/reference/packages.html)
- [DNS](115.159.19.22)
- [知道](http://stackoverflow.com/)

##2，ViewGroup: 
- **LinearLayout**               可以设置横向排列(Horizontal row),竖向排列(Vertical column)。
- **RelativeLayout**             将子视图与父布局相对排列，或者子视图相对子视图排列。

##3，LayoutParams:
属性带"layout_"字的表示布局参数，由父View使用。
 


- `android:layout_width="150dp"`dp是密度无关像素，按钮至少要48dps.
- `android:layout_height="wrap_content"`自适应内容的宽度和高度
- `android:layout_height="match_parent"`以父标签匹配

 **LinearLayout**

- `android:layout_weight="1"`                    //布局权重，占用父View未分配空间的比例

**RelativeLayout:**      
视图组合布局参数。值默认为false,View默认放置在左上角。可以组合使用。可搜索RelativeLayout.LayoutParams获得更多帮助。

- `android:layout_alignParentTop="true"`         其值为 true表示与上沿的父视图对齐，false表示不与父视图上沿对齐
- `android:layout_alignParentDown="true"`下沿对齐
- `android:layout_alignParentLeft="true"`        //左边对齐
- `android:layout_alignParentRight="true"`       //右边对齐
- `android:layout_centerHorizontal="true" `      //设置为真，表示水平居中显示。
- `android:layout_centerVertical="true"`         //设置为真表示垂直居中放置。
- `android:layout_toleftOf="@id/idname"`         //放置在idname的左边。
- `android:layout_above="@id/idname"`            //放置在idname的上方。
- `android:layout_margin="8dp"`                  //子View边框到父View边框的距离。由父View处理边距。
- `android:layout_marginLeft="8dp" `          //material design标准规定边距以8dp的倍数递整。左边距起始在16dp.
- `android:layout_marginRighr="8dp"`          //material design标准规定边距以8dp的倍数递整。左边距起始在16dp.
- `android:layout_marginTop="8dp"`
- `android:layout_marginBottom="8dp"`

##4，属性：
- `android:background="@android:color/darker_gray"`   //背景颜色，查找
- `android:id="@+id/ben_text_view"`        //@指资源名是ID。+号表示第一次定义。/后面是ID名称。
- `android:padding="8dp"`                  //体外边框到其所在的View边框的距离。由子View处理边距。
- `android:paddingLeft="8dp"`           //默认0dp.属性可设置在父类，就多了一个外边框。
- `android:paddingRight="8dp"`          //material design标准规定边距以8dp的倍数递整。左边距起始在16dp.
- `android:paddingTop="8dp"` 
- `android:paddingBottom="8dp"`
- `xmlns:android="http://schemas.android.com/apk/res/android"`  //指定命名空间，可以指定自己的命名空间避免名字的冲突。

   **LinearLayout**



- `android:orientation="vertical"`         //决定布局是一行还是一列。有horizontal和vertical两个值. 
  
 **TextView**

- `android:text="Hapy Birthday"`           //不检测文字的内容。
- `android:textColor="#3F51B5"`            //背景颜色指定值通过Material Design规范来查找
- `android:TextSize="45sp"`                //sp是比例无关像素的缩写，大小使用Material Design规范。
- `android:textAllCaps="true"`             //通过设计文档来搜索cap查找说明
- `android:textStyle="bold"`               //通过设计文档来搜索bold来查找说明
- `android:textAppearance="?android:textAppearanceLarge"`      //使用android内部规范。
 
  **ImageView**

- `android:src="@drawable/cake"`           //不用指定图片的扩展名，自动识别。
- `android:scaleType="center"`             //缩放属性，无缩放。
- `android:scaleType="centerCrop"`          //按图片比例缩放，填充屏幕。按图片中间进行裁减。

##5，快捷键：


- 撤消：Ctrl+z
- 重做：Ctrl+Shift+z
