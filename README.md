# Mac-Android-Studio-use-Svn-Github

Mac中Android Studio的svn使用笔记
•	Add Ignored
•	Share project
•	Checkout project 
•	Update project 

•	一、Add Ignored
AS  preferences  version control  Ignored files   “+” 
{
1.specified file     local.properties
2.all files under  .gradle  .idea  build
3.all files matching  *.iml
}

二、share project
VCS  import into version control  share project(subversion)  弹出选项卡  “+”   选择地址  选择1.6Format  输入SVN账号密码  ok

此时项目代码并没有提交到svn上；黄色文件 为省略文件，绿色文件为待提交的文件

VCS↑上传  选择要上传文件  点击上传同步按钮（或者一步到位，勾选右侧，auto – update after commit）

上传一分钟后，弹出框提示      选择commit提交完毕
{
commit 提交
cancel 取消
review 查看远程服务项目
}

三、checkout project
AS启动页   VCS  Subversion   弹出框 Repositeries “+”  增加SVN的地址路径   填写svn权限  选择本地存储目录    设置选项（默认）  选择1.6Format  成功checkout   ok开启项目

       
四、update project 
项目右键  Subversion   commit file 提交



Mac中Android Studio 的GitHub 使用
•	Add Ignored
•	GitHub User Login
•	Share project
•	Checkout project 
•	Update project 

•	一、Add Ignored
AS  preferences  version control  Ignored files   “+” 
{
1.specified file     local.properties
2.all files under  .gradle  .idea  build
3.all files matching  *.iml
}

二、GitHub User Login
AS  preferences  version control  GitHub   ok
{
     Host Login Password Timeout     使用测试
}

三、share project
VCS  import into version control  share project(GitHub)  弹出选项卡   share
{
New repository name 
Description  
private
}

  选择上传文件/Commit  Message   提交Ok

四、checkout project
AS启动页   VCS  GitHub   弹出框  
{
   Git Repository Url 
   Parent directory 
   Directory Name
}

 Unregistered VCS ROOT  
{
ADD ROOT 
CONFIGURE 
IGNORE
}

 选择Unregistered root   ok
       
五、update project 
项目右键/VCS   Git   add/commit file   push
