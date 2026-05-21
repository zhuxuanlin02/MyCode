<div align="center">

# MyCode Python 

### 个人终端 AI 编程助手
[![Python](https://img.shields.io/badge/python-3.11-blue)]()

</div>

---

## 🚀 快速开始

```bash
# 安装
pip install -e .

# 运行
python -m minicode.main
```

## ⚙️ 配置

### 设置文件

`~/.mini-code/settings.json`：

```json
{
  "model": "claude-sonnet-4-20250514",
  "env": {
    "ANTHROPIC_BASE_URL": "https://api.anthropic.com",
    "ANTHROPIC_AUTH_TOKEN": "your-token-here"
  }
}
```
## 🎯 核心特性

- **🖥️ 丰富的终端 UI** — 备用屏幕 TUI，面板、ANSI 样式、平滑滚动
- **🤖 智能代理循环** — 多轮工具使用，自动规划、执行、迭代
- **🛠️ 30+ 内置工具** — 文件 I/O、代码搜索、Shell、Git、测试等
- **🔒 权限系统** — 审批、拒绝、自动允许工具调用
- **💾 会话持久化** — 保存并恢复对话，30 秒自动保存
- **🧠 三级记忆** — 对话 → 会话 → 长期记忆
- **🔌 MCP 集成** — 连接外部模型上下文协议服务器
- **⌨️ 斜杠命令** — `/help`、`/tools`、`/cost`、`/config`、`/context`、`/memory`

---

## 🛠️ 内置工具

### 文件操作
| 工具 | 说明 |
|---|---|
| `list_files` | 列出目录内容 |
| `grep_files` | 跨文件正则搜索 |
| `read_file` | 读取文件（支持行范围） |
| `write_file` | 创建或覆盖文件 |
| `edit_file` / `patch_file` | 文件编辑 |

### 代码智能
| 工具 | 说明 |
|---|---|
| `find_symbols` | AST 符号搜索 |
| `find_references` | 查找符号引用 |
| `code_review` | 代码质量分析 |

### 执行与测试
| 工具 | 说明 |
|---|---|
| `run_command` | 执行 Shell 命令 |
| `test_runner` | 测试发现和执行 |

### DevOps
| 工具 | 说明 |
|---|---|
| `git` | Git 工作流 |
| `docker_helper` | Docker 管理 |
| `db_explorer` | SQLite 数据库探索 |

