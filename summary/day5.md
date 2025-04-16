Day 5（2025.04.13）: Shell脚本入门  
学习内容：  
Shell脚本基础：`#!/bin/bash`、变量、`if`判断  
实践任务:  
- 编写脚本`backup.sh`：自动将指定目录备份到`/backup`并打时间戳
- 示例代码:  
    #!/bin/bash
    cp -r $1 /backup/$(date +%Y%m%d)`

笔记：  
🌟 今日核心任务  
1. 掌握 Shell 脚本基础语法  
2. 编写自动备份脚本 `backup.sh`   

📜 Shell 脚本基础  
1. 脚本结构  
- Shebang 行：`#!/bin/bash` 声明 Bash 解释器  
- 变量定义：`name="value"`（等号两侧无空格）  
- 使用变量：`$name` 或 `${name}`  
 2. 条件判断 (`if`) 
if [ 条件 ]; then
    # 执行命令
fi  
常用条件：  
- `-d 目录`：检查目录是否存在  
- `-f 文件`：检查文件是否存在  
- `$# -eq 0`：检查是否有参数输入  

🚀 扩展  
1. **压缩备份**：用 `tar` 减少占用空间
2. **定时任务**：通过 `crontab` 每日自动备份
选项：
-e后在文件尾部添加新定时任务
-l浏览该用户拥有的定时任务

⚠️ 注意事项  
1. Shebang 行必写：确保脚本用 Bash 执行。  
2. 变量赋值无空格：`name="value"` 错误写法 `name = "value"`。  
3. 路径安全检查：避免备份目录嵌套在源目录内（参考 `[[ "$backup" == "$source"/* ]]`）。
4. 添加执行权限：`chmod +x script.sh`  

资源:  
[Shebang 解释]  
https://bash.cyberciti.biz/guide/Shebang  
[Bash 脚本教程]  
https://wangdoc.com/bash/  
[Shell Scripting Tutorial]  
https://www.shellscript.sh/
