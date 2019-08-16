# [JavaBridge教程](https://javabridge.xcgzs.xyz)
## 基本代码框架
### 项目清单
```
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="应用包名" >
    <application
        android:allowBackup="true"
        android:icon="应用图标路径"
        android:label="应用名称"
        android:theme="应用主题" >
        <activity
            android:name="启动类" 
            android:label="应用名称" >
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />
                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>
</manifest>
```
###### 应用图标路径根据自己情况设定，图标在res文件夹中时路径一般写@drawable/ic_launcher；应用名称自己写，然后应用主题在后面教程里会讲到。
### Java文件
```
package com.javabridge; //这里写应用包名

import com.google.appinventor.components.runtime.*;

public class Screen1 extends Form
{
    声明部分
    protected void $define()
    {
        this.Title("应用标题");
        初始化执行部分
    }
}

```
##### **声明部分**用来声明变量或者声明组件对象等。
```
声明格式：private 对象 对象名称;
变量声明：private 数据类型 变量名称;
创建按钮：private Button Button1 = new Button(this);
创建变量：private int a = 0;
//创建组件时后面括号中写容器，表示这个组件创建在哪个容器中，
而小部分组件不需要写容器，后面会讲到。
```

##### **初始化执行部分**用来给变量赋值，设置组件属性等。
```
this.Title("Screen1");
Btoon1.Text("Button1text");
```

 
