# activity2
安卓实验2
**1、线性布局代码:**
```java
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:paddingLeft="1dp"
    android:paddingRight="1dp"
    android:background="#000000"
    android:orientation="vertical" >
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:orientation="horizontal">
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:background="#000000"
            android:layout_weight="1"
            android:text="one,one"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1.5"
            android:background="#000000"
            android:text="one,two"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="one,three"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="one,four"
            android:textColor="#FFFFFF"/>
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:orientation="horizontal">
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="two,one"
            android:textColor="#FFFFFF" />
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1.5"
            android:background="#000000"
            android:text="two,two"
            android:textColor="#FFFFFF"/>

        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="two,three"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="two,four"
            android:textColor="#FFFFFF"/>
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:orientation="horizontal">
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="three,one"
            android:textColor="#FFFFFF" />
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="three,two"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="three,three"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="three,four"
            android:textColor="#FFFFFF"/>
    </LinearLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:orientation="horizontal">
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="four,one"
            android:textColor="#FFFFFF"
            />
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1.4"
            android:background="#000000"
            android:text="four,two"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="four,three"
            android:textColor="#FFFFFF"/>
        <Button
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:background="#000000"
            android:text="four,four"
            android:textColor="#FFFFFF"/>
    </LinearLayout>

</LinearLayout>
```

**线性截图：**

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190331213206718.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dhbmdiaW5fMTAxMg==,size_16,color_FFFFFF,t_70)


**2、ConstraintLayout代码：**
```java
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#000000"
    android:orientation="vertical" >
    xmlns:app="http://schemas.android.com/apk/res-auto">

    <RelativeLayout
        android:layout_width="match_parent"
        android:layout_height="90dp"
        android:orientation="horizontal">

        <TextView
            android:id="@+id/tv1"
            android:layout_width="60dp"
            android:layout_height="60dp"
            android:layout_margin="0dp"
            android:background="#ff0000"
            android:gravity="center"
            android:text="red" />

        <TextView
            android:id="@+id/tv2"
            android:layout_width="90dp"
            android:layout_height="60dp"
            android:layout_alignParentTop="true"
            android:layout_alignParentEnd="true"
            android:layout_marginTop="0dp"
            android:layout_marginEnd="148dp"
            android:background="#ffa500"
            android:gravity="center"
            android:text="orange" />

        <TextView
            android:id="@+id/tv3"
            android:layout_width="90dp"
            android:layout_height="60dp"
            android:layout_alignParentStart="true"
            android:layout_alignParentTop="true"
            android:layout_marginStart="294dp"
            android:layout_marginTop="0dp"
            android:background="#ffff00"
            android:gravity="center"
            android:text="yellow" />
    </RelativeLayout>

    <RelativeLayout
        android:layout_width="match_parent"
        android:layout_height="90dp"
        android:orientation="horizontal">

        <TextView
            android:id="@+id/tv4"
            android:layout_width="80dp"
            android:layout_height="60dp"
            android:layout_alignParentStart="true"
            android:layout_alignParentTop="true"
            android:layout_marginStart="66dp"
            android:layout_marginTop="0dp"
            android:background="#008000"
            android:gravity="center"
            android:text="green" />

        <TextView
            android:id="@+id/tv5"
            android:layout_width="70dp"
            android:layout_height="60dp"
            android:layout_alignParentStart="true"
            android:layout_alignParentTop="true"
            android:layout_marginStart="155dp"
            android:layout_marginTop="0dp"
            android:background="#0000ff"
            android:gravity="center"
            android:text="blue" />

        <TextView
            android:id="@+id/tv6"
            android:layout_width="80dp"
            android:layout_height="60dp"
            android:layout_alignParentStart="true"
            android:layout_alignParentTop="true"
            android:layout_marginStart="233dp"
            android:layout_marginTop="0dp"
            android:background="#4b0082"
            android:gravity="center"
            android:text="indigo" />


    </RelativeLayout>
    <RelativeLayout
        android:layout_width="match_parent"
        android:layout_height="60dp"
        android:orientation="horizontal">
        <TextView
            android:id="@+id/tv7"
            android:layout_width="400dp"
            android:layout_height="60dp"
            android:layout_margin="0dp"
            android:background="#ee82ee"
            android:gravity="center"
            android:text="violte"/>
    </RelativeLayout>
</LinearLayout>
```
**ConstraintLayout截图：**
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190331214555990.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dhbmdiaW5fMTAxMg==,size_16,color_FFFFFF,t_70)


**3、表格布局代码**
```java
<?xml version="1.0" encoding="utf-8"?>
<TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:stretchColumns="*"
    >

    <TableRow>
        <TextView
            android:textColor="#000000"
            android:layout_marginLeft="10dp"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="Open..." />
        <TextView
            android:textColor="#000000"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_gravity="right"
            android:text="Ctrl-O" />


    </TableRow>

    <TableRow>

        <TextView
            android:textColor="#000000"
            android:layout_marginLeft="10dp"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="left"
            android:text="Save..." />

        <TextView
            android:textColor="#000000"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="right"
            android:text="Ctrl-S" />
    </TableRow>

    <TableRow>

        <TextView
            android:textColor="#000000"
            android:layout_marginLeft="10dp"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="left"
            android:text="Save As..." />

        <TextView
            android:textColor="#000000"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:gravity="right"
            android:text="Ctrl-Shift-S" />
    </TableRow>
    <View
        android:layout_width="match_parent"
        android:layout_height="5px"
        android:background="#000000"/>
    <TableRow>

        <TextView
            android:textColor="#000000"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="left"
            android:text="X Import..." />
    </TableRow>
    <TableRow>

        <TextView
            android:textColor="#000000"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="left"
            android:text="X Emport..." />

        <TextView
            android:textColor="#000000"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:gravity="right"
            android:text="Ctrl-E" />
    </TableRow>
    <View
        android:layout_width="match_parent"
        android:layout_height="5px"
        android:background="#000000"/>
    <TableRow>

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="left"
            android:layout_margin="10dp"
            android:text="Quit"
            android:textColor="#000000" />
    </TableRow>
</TableLayout>
```
**截图：**![在这里插入图片描述](https://img-blog.csdnimg.cn/20190331214953321.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3dhbmdiaW5fMTAxMg==,size_16,color_FFFFFF,t_70)
