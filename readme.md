---
title:Android布局实验
tags: JAVA,面向对象,基础
---

## 实验一

![enter description here][1]

#### 部分代码
```java
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#000000"
    >

    <LinearLayout android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        android:weightSum="1">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="ONE,ONE"
            android:textColor="#ffffff"
            android:layout_margin="2dp"/>

        <Button
            android:id="@+id/button"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_margin="2dp"
            android:background="@drawable/butten_border_color"
            android:text="ONE,TWO"
            android:textColor="#ffffff"
            android:layout_weight="1.45" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="ONE,THREE"
            android:textColor="#ffffff"
            android:layout_margin="2dp"/>
            />
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="ONE,FOUR"
            android:textColor="#ffffff"
            android:layout_margin="2dp"/>
    </LinearLayout>

    <LinearLayout android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        android:weightSum="1">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="TWO,ONE"
            android:textColor="#ffffff"
            android:layout_margin="2dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="TWO,TWO"
            android:textColor="#ffffff"
            android:layout_margin="2dp"
            android:layout_weight="1.45" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="TWO,THREE"
            android:textColor="#ffffff"
            android:layout_margin="2dp"/>
        />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="TWO,FOUR"
            android:textColor="#ffffff"
            android:layout_margin="2dp"/>
    </LinearLayout>

    <LinearLayout android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        android:weightSum="1">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="THREE,ONE"
            android:textColor="#ffffff"
            android:layout_margin="2dp"
            android:layout_weight="0.63" />
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="THREE,TWO"
            android:textColor="#ffffff"
            android:layout_margin="2dp"/>

        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="THREE,THREE"
            android:textColor="#ffffff"
            android:layout_margin="2dp"/>
        />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="THREE,FOUR"
            android:textColor="#ffffff"
            android:layout_margin="2dp"/>
    </LinearLayout>

    <LinearLayout android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        android:weightSum="1">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="FOUR,ONE"
            android:textColor="#ffffff"
            android:layout_margin="2dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="FOUR,TWO"
            android:textColor="#ffffff"
            android:layout_margin="2dp"
            android:layout_weight="1.45" />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="FOUR,THREE"
            android:textColor="#ffffff"
            android:layout_margin="2dp"/>
        />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:background="@drawable/butten_border_color"
            android:text="FOUR,FOUR"
            android:textColor="#ffffff"
            android:layout_margin="2dp"/>
    </LinearLayout>

</LinearLayout>

```
#### 实验截图

![enter description here][2]

## 实验二
![enter description here][3]


#### 部分代码
```java
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#000000">
    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="RED"
        android:textColor="#000000"
        android:layout_alignParentLeft="true"
        android:background="#FF0000"/>
    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="YELLOW"
        android:layout_alignParentRight="true"
        android:textColor="#000000"
        android:background="#FFFF00"/>
    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:id="@+id/orange"
        android:text="ORANGE"
        android:layout_centerHorizontal="true"
        android:textColor="#000000"
        android:background="#FFA500"/>
    <Button
        android:layout_width="70dp"
        android:layout_height="wrap_content"
        android:id="@+id/blue"
        android:text="BLUE"
        android:layout_below="@+id/orange"
        android:layout_centerHorizontal="true"
        android:textColor="#000000"
        android:background="#0000FF"
        android:layout_marginTop="20dp"
        android:layout_marginBottom="20dp"
        android:layout_marginLeft="10dp"
        android:layout_marginRight="10dp"/>

    <Button
        android:layout_width="70dp"
        android:layout_height="wrap_content"
        android:layout_alignBottom="@+id/blue"
        android:layout_toLeftOf="@+id/blue"
        android:background="#008000"
        android:text="GREEN"
        android:textColor="#000000" />

    <Button
        android:layout_width="70dp"
        android:layout_height="wrap_content"
        android:layout_alignBottom="@+id/blue"
        android:layout_toRightOf="@+id/blue"
        android:background="#4B0082"
        android:text="INDIGO"
        android:textColor="#000000" />
    <Button
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_centerHorizontal="true"
        android:layout_below="@+id/blue"
        android:background="#EE82EE"
        android:text="VIOLET"
        android:textColor="#000000" />
</RelativeLayout>
```
#### 实验截图

![enter description here][4]

## 实验三

![enter description here][5]

#### 部分代码
```java
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:background="#000000">



    <TableLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="#FFFFFF"
        android:textAllCaps="false"
       >

        <Button
            android:layout_width="wrap_content"
            android:layout_height="29dp"
            android:background="#000000"
            android:text="     open...                                                                      ctrl-o"
            android:textColor="#FFFFFF"
            android:textAllCaps="false"/>
        <Button
            android:textAllCaps="false"
            android:layout_width="wrap_content"
            android:layout_height="29dp"
            android:background="#000000"
            android:text="     save...                                                                       ctrl-s"
            android:textColor="#FFFFFF"/>
        <Button
            android:textAllCaps="false"
            android:layout_width="wrap_content"
            android:layout_height="29dp"
            android:background="#000000"
            android:text="     save as...                                                        ctrl-shift-o"
            android:textColor="#FFFFFF"/>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="2dp"
            android:background="#ffffff" />
        <Button
            android:textAllCaps="false"
            android:layout_width="wrap_content"
            android:layout_height="29dp"
            android:background="#000000"
            android:text="X  Import...                                                                            "
            android:textColor="#FFFFFF"/>
        <Button
            android:textAllCaps="false"
            android:layout_width="wrap_content"
            android:layout_height="29dp"
            android:background="#000000"
            android:text="X  Export...                                                                  ctrl-e"
            android:textColor="#FFFFFF"/>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="2dp"
            android:background="#ffffff" />
        <Button
            android:textAllCaps="false"
            android:layout_width="wrap_content"
            android:layout_height="29dp"
            android:background="#000000"
            android:text="Quit...                                                                           "
            android:textColor="#FFFFFF"/>


    </TableLayout>


</LinearLayout>
```
#### 实验截图

![enter description here][6]


  [1]: ./1.png "1"
  [2]: ./2.png "2"
  [3]: ./3.png "3"
  [4]: ./4.png "4"
  [5]: ./5.png "5"
  [6]: ./6.png "6"