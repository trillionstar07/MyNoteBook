### 首先到andriod目录的platform-tools 下打开adb工具

cd /Users/trillion-star/Library/Android/sdk/platform-tools/

### 使用adb shell命令运行adb

adb shell

### 在弹出来的命令提示中输入如下命令

emulator64_arm64:/ $ su

### 找到messaging的数据库

emulator64_arm64:/ # cd data/data/com.google.android.apps.messaging/

## cd到数据库

cd databases/

然后输入sqlite3 bugle_db  

### 然后再sqlite提示中输入

.table 

### 然后输入 select * from conversations







