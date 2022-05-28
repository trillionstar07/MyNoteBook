mac adb环境变量配置：



1. 启动终端，进入当前用户的HOME目录，命令如下：

   

   ```bash
   cd $HOME
   ```

   ### 2. 更新.bash_profile文件（当该文件存在时），如果该文件不存在，可通过如下命令创建：

   ```css
   touch .bash_profile
   ```

   ### 3. 打开.bash_profile文件，对其内容进行编辑，命令如下：

   ```css
   open -e .bash_profile
   ```

   ### 4. 此时文本编辑器会打开一个文本，编辑内容如下：

   ```ruby
   export PATH=${PATH}:/Users/Trillion-Star/Library/Android/sdk/platform-tools
   export PATH=${PATH}:/Users/Trillion-Star/Library/Android/sdk/tools
   ```

   ### 5. 保存文件，关闭.bash_profile,更新刚配置的环境变量，命令如下：

   ```bash
   source .bash_profile
   ```

   ### 6. 解决mac重启配置的adb命令不生效问题：

   6.1创建 ~/.zshrc文件

   ```undefined
   touch ~/.zshrc
   ```

   6.2 打开 ~/.zshrc文件

   ```kotlin
   open ~/.zshrc
   ```

   6.3 向 ~/.zshrc文件 追加写入以下内容：保存退出即可

   ```bash
   source .bash_profile
   ```

   