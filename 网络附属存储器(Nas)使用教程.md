# 网络附属存储器(Nas)使用教程

本教程编写：2351610105方泽宇，有问题请联系1139950253@qq.com，对于较为简单的问题，我将会在24小时内回复。

本教程所有用作示例的ip均为内网ip，请根据教程指示对内容进行替换

## Windows操作系统下SMB映射协议

SMB协议（Server Message Block，服务器消息块）是一种网络通信协议，主要用于共享文件、打印机和其他资源。smb协议可以将Nas的磁盘空间像电脑硬盘一样映射到此电脑(Windows7及以下版本为“计算机”)，对文件进行读写操作。

### Windows系统下，使用smb映射网络存储器的具体操作步骤如下

1. 在桌面/文件资源管理器左侧找到“网络”并右击。
2. 在弹出的选项卡中，左键选择“映射网络驱动器”。
3. 在“驱动器”选项卡中选择一个没有冲突的盘符，一般为Z。在“文件夹”选项卡中，输入Nas管理员提供的链接。注意，链接中所有的"/"需要改写为"\\"；由于Windows系统限制，在ip地址的"\\"后面一定还有一个"\\"。

<img src="https://i.imgur.com/Y20wnsj.png" style="zoom: 80%;" />

4. 然后点击“完成”，即可在“此电脑”内看到相应盘符。

## Mac、Linux桌面版系统下使用SMB映射协议

### MacOS、Linux系统下，使用smb映射网络存储器的具体操作步骤如下

1. 修改Nas管理员提供的ip地址，将其改写为:smb://ip/的形式。例如:192.168.31.168，可以被改写为smb://192.168.31.168.

2. 对于Mac系统，笔者没有MacBook等相关设备，所以下图为网图。打开访达，在左上角菜单栏中依次点击“Go-Connect to sever(连接到服务器)"，输入smb://192.168.31.168，即可完成映射。

<img src="https://img.php.cn/upload/article/000/887/227/168143336579455.png" alt="Mac-Finder-Connect-to-Server-Option" style="zoom:80%;" />

3. 对于Linux发行版，不同发行版有不同的连接方式，常见的思路即为将smb://192.168.31.168写到某一个框中即可。鉴于Linux系统多为专业用户，这边不做详细介绍。

## iPadOS、IOS系统下，使用SMB映射协议

### iPadOS、IOS系统下，使用smb映射网络存储器的具体操作步骤如下

1. 同上。修改Nas管理员提供的ip地址，将其改写为:smb://ip/的形式。例如:192.168.31.168，可以被改写为smb://192.168.31.168.
2. 打开”文件“app。
3. 轻点右上角三点，选择"Connect to sever(连接到服务器)"。

4. 在Server选项卡中填写修改好的链接即可。

<img src="https://i.imgur.com/EM8McZ7.png" alt="image-20240521221624798" style="zoom: 25%;" />

## 其他安卓操作系统的操作方法

### 类似iPadOS/IOS，不做过多赘述



# 更新日志

##### 本教程首次发布于2024-05-21，修订于2024-05-21

##### 2024-05-21首次修订——方泽宇(1139950253@qq.com)