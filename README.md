## skills

## tmux

多数 agent harness 没有持久 shell，没有真正意义上的“terminal tool”

在 LLM 操作终端的时候只能输入一个命令，拿到一段响应，而不能做持续性，交互式的操作

- 对于长程编译，不能“盯着日志，走偏就修”
- 不能进入一台 SSH 机器然后保持长连接
- 不能 source venv
- 不能 apt install 然后“按 y”
- 不能操作 gdb
- 不能 devcontainer exec bash 进入开发容器环境

这个 skill 对以上场景做了优化，还附带 tmux 的其他好处：

- 可以同时开多终端，多标签，区分 session 和 window
- agent 工作时，人类可以随时 `tmux attach-session` 来监视，介入整个终端

## self-reflection

解决 AI 胡说八道、遗漏事实的问题。

每次都要骂回去，很麻烦，所以用这个 skill 让 AI 自己骂自己。

## solution-research

大多数问题，肯定已经有很多开源方案，但太多方案了，不知道怎么选。

让 AI 自己去深入每个方案，比较技术路线和源码。

## max-research

经常莫名其妙想研究一个话题，但现有的 Deep Research 不能满足我的需求。

希望它找遍互联网的每一个角落，也许就能找到一点线索。
