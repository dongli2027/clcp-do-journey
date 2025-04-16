Day 2（2025.04.10）: 文件操作进阶
学习内容：  
- 文件操作：cp, mv, rm, cat, echo  
- 文本编辑：nano或vim基础（只需学会保存退出即可）  
实践任务：  
- 将`hello.txt`复制到新目录`backup`，并重命名为`hello_backup.txt`  
- 用`echo "Hello Linux" >> hello.txt`追加内容  
小技巧：  
- 使用`tab`键自动补全路径，`Ctrl+C`强制终止当前命令

笔记: 
🔑 核心内容  
1. 文件操作
- cp file dir/ → 复制文件  
- mv file new_name → 重命名/移动  
- rm file → 删除文件⚠️不可逆！）  
- cat file → 查看内容  
- echo "text" >> file → 追加内容（`>`覆盖）  

3. 文本编辑器  
- Nano：直接编辑 → `Ctrl+O`保存 → `Ctrl+X`退出  
- Vim：`i`进入编辑 → `Esc` → `:wq`保存退出

3.Vim退出 🚪
* 狂按 `Esc`（确保进入命令模式）
*   
  - 保存退出→ :wq
  - 强制退出→ :q!
  - 未修改退出→ :q
  - 仅保存暂不退出→ :w
＊ 按回车执行 

资源：  
[全基础命令权威解释文档]   
https://www.gnu.org/software/coreutils/manual/coreutils.html  
[nano 快速指南]  
https://www.nano－editor.org/dist/latest/cheatsheet.html    
[命令速查表]  
https://cheatography.com/davechild/cheat-sheets/linux-command-line/
