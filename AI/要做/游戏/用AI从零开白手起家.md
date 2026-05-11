## Claude Code 与 Roblox Studio MCP 的深度联动
https://mp.weixin.qq.com/s/mV22b2PRDXrHKu5rAoC3Uw

```
54个终端指令，完全脱离Studio图形界面手动操作。

# Step 1 — Install the MCP server
claude mcp add robloxstudio -- npx -y robloxstudio-mcp@latest

# Step 2 — Download the Studio plugin
curl -L "https://github.com/boshyxd/robloxstudio-mcp/releases/download/v2.5.1-plugin-fix/MCPPlugin.rbxmx" \
  -o ~/Documents/Roblox/MCPPlugin.rbxmx
随后在Roblox Studio端完成三步配置：

将插件安装至文档目录
在游戏设置中开启HTTP请求权限
通过Claude执行get_place_info，返回项目名即表示连接成功
核心配置文件：CLAUDE.md
缺少此文件，AI极易输出JavaScript或标准Lua 5.1代码，甚至导致游戏一键崩溃。该文件用于明确界定AI的运行环境：

# CLAUDE.md — paste this in your project root

## Language
This project uses Luau (not Lua, not JavaScript, not TypeScript).
Always write strict Luau with type annotations.

## Architecture
- Server scripts: ServerScriptService/
- Client scripts: StarterPlayerScripts/
- Shared modules: ReplicatedStorage/Modules/
- Use RemoteEvents for ALL client-server communication
- Use DataStoreService for ALL persistent data (never client-side)

## Roblox Services
Always use game:GetService() pattern:
local Players = game:GetService("Players")
local DataStoreService = game:GetService("DataStoreService")
local ReplicatedStorage = game:GetService("ReplicatedStorage")

## Rules
- Server-side validation on all currency transactions
- Never trust the client for any game state
- Use pcall() for all DataStore operations
- Use task.spawn() not coroutine.wrap()
```

## 用AI从零开白手起家
https://mp.weixin.qq.com/s/7ZnaPVhk0E5V8nFuukIqDw
