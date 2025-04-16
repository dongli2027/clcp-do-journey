Day 4（2025.04.12）: 进程管理与Python联动  
学习内容：  
- 进程查看：`ps`, `top`, `kill`
- 运行Python脚本：`python3 your_script.py`  
实践任务：  
- 写一个简单的Python脚本（如打印当前时间），在Linux中运行  
- 用`nohup`让脚本后台运行，并用`ps`查看进程  

笔记： 
🔑 核心知识点 
1. 进程管理  
- `ps aux` → 查看所有进程  
- `top` → 实时监控资源（按 `q` 退出）或增强版`htop` （按`F10`退出）  
- `kill -9 [PID]`或`pkill -9 [进程名]` → 强制终止，默认传递-9可省  
2. Python 脚本运行  
- 前台：`python3 脚本名.py`  
- 后台：`nohup python3 -u 脚本名.py > 日志.log &`  

⚠️ **附加提示**  
- `nohup` 必须搭配 `&` 使用 → 后台运行让出终端  
- 及时输出后续结果：nohup后+`-u` （禁用python缓冲）参数
或 脚本中+`flush=True`  （强制刷新）
- 查找 PID：`pgrep [进程名]"`  

资源：  
[Linux Command Library (建议使用搜索查找目标命令)]  
https://linuxcommandlibrary.com/   
[DigitalOcean 进程管理教程]  
https://www.digitalocean.com/community/tutorials/how-to-use-ps-kill-and-nice-to-manage-processes-in-linux  
[Python 时间格式化代码表]  
https://strftime.org/
