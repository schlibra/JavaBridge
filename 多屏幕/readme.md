### 在项目清单中添加新的启动类：
```
  <activity android:name="启动类">
            <intent-filter>
                <action  android:name="android.intent.action.MAIN"/>
            </intent-filter>
        </activity>
```
### 打开屏幕但不带初始值：
```
startActivity(new Intent().setClass(this, 屏幕名称.class));
```
### 打开屏幕并带初始值：
```
startActivity(new Intent().setClass(this,屏幕名称.class).putExtra("startValue","初始值"));
```
### 获取初始值：
```
getIntent().getExtras().get("startValue");
```
### 关闭屏幕(传值教程下次再加入)：
```
finish();
```
### 退出程序：
```
system.exit(1);
```





