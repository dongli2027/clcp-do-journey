Day 3（2025.04.11）: 用户权限管理  
学习内容：  
- 用户与组：`sudo`, `useradd`, `chown`, `chmod`  
- 理解权限符号（如`rwx`）和数字表示（如`755`）  
实践任务：  
新建一个用户`testuser`，并修改`hello.txt`的权限为仅该用户可读写  
注意：  
权限问题可能导致“Permission denied”，学会用`ls -l`查看当前权限  

笔记:  
🌟 核心任务 
1. 掌握用户与组管理命令  
2. 理解文件权限符号与数字  
3. 完成用户创建及权限修改实践
 
📚 关键知识点  
🔑 用户与组管理  
- sudo：临时获取管理员权限（需输入密码）  
- useradd -m：创建用户并生成家目录（无 `-m` 会导致无家目录）  
- passwd：为用户设置登录密码  
- groups：查看用户所属组  

🔑 文件权限控制  
权限符号：  
`r` = 读（4） / `w` = 写（2） / `x` = 执行（1）   
权限命令：  
- `chown 用户:组 文件`**：修改所有者（需 `sudo`）  
- `chmod 权限值 文件`**：直接设置权限

资源:  
[红帽官方权限文档]  
https://www.redhat.com/sysadmin/linux-file-permissions-explained  
[菜鸟教程-Linux权限]  
https://www.runoob.com/linux/linux-file-attr-permission.html
