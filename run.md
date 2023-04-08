# tmux commands
tmux ls  # 查看当前 Tmux 会话
tmux new -s <session-name>  # 新建会话
tmux attach -t <session-name>  # 接入会话
# tmux attach -t mlp_c
# 分离回话！！！
tmux detach  # 可在命令行输入时
直接关闭窗口  # 模型运行，不可在命令行输入时
tmux kill-session -t <session-name>  # 杀死会话
tmux rename-session -t <old-name> <new-name>  # 重命名会话

# 杀内存
fuser -v /dev/nvidia*
kill -9 ...