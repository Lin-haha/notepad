# 添加时间戳
1.首先找到noteslist_item.xml布局文件，是笔记每个条目的布局，原码为：
```
<RelativeLayout android:layout_height="match_parent"
    android:layout_width="match_parent"
    xmlns:android="http://schemas.android.com/apk/res/android">
    <TextView xmlns:android="http://schemas.android.com/apk/res/android"
        android:id="@android:id/text1"
        android:layout_width="match_parent"
        android:layout_height="?android:attr/listPreferredItemHeight"
        android:textAppearance="?android:attr/textAppearanceLarge"
        android:gravity="center_vertical"
        android:paddingLeft="5dip"
        android:singleLine="true"
    />
</RelativeLayout>
```
修改后将时间戳显示在每个笔记条目中，修改后的代码为：
```
<RelativeLayout android:layout_height="match_parent"
    android:layout_width="match_parent"
    xmlns:android="http://schemas.android.com/apk/res/android">
    <TextView xmlns:android="http://schemas.android.com/apk/res/android"
        android:id="@android:id/text1"
        android:layout_width="match_parent"
        android:layout_height="?android:attr/listPreferredItemHeight"
        android:textAppearance="?android:attr/textAppearanceLarge"
        android:gravity="center_vertical"
        android:paddingLeft="5dip"
        android:singleLine="true"
    />
    <TextView
        android:id="@+id/text2"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:paddingLeft="5dip"
        android:singleLine="true"
        android:gravity="center_vertical"
    />
</RelativeLayout>
```




# 实验截图
运行手机截图：

![展示图](https://github.com/Lin-haha/notepad/blob/master/photo/3.png)
![展示图](https://github.com/Lin-haha/notepad/blob/master/photo/phone.png)



工作台截图：

![展示图](https://github.com/Lin-haha/notepad/blob/master/photo/2.png)
