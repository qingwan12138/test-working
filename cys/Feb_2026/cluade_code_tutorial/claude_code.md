# Claude Code 接入 GLM-5 配置指南

本指南介绍如何配置 Claude Code 使用智谱AI的 GLM-5 大模型。

## 前提条件

- **Node.js**: 18 或更高版本
- **智谱AI API Key**: 从 [智谱AI开放平台](https://open.bigmodel.cn/) 或者从咸鱼获取

## 安装 Claude Code

```bash
npm install -g @anthropic-ai/claude-code
```

## 配置 GLM-5

选择以下任意一种方式配置环境变量。

### 手动配置（全平台）

编辑配置文件 `~/.claude/settings.json`，添加以下内容：

```json
{
    "env": {
        "ANTHROPIC_AUTH_TOKEN": "your_zhipu_api_key",
        "ANTHROPIC_BASE_URL": "https://open.bigmodel.cn/api/anthropic/",
        "API_TIMEOUT_MS": "3000000",
        "CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC": 1
    }
}
```

> 将 `your_zhipu_api_key` 替换为你的智谱 API Key

配置后需**新建命令行窗口**才能生效。

## 环境变量说明

| 环境变量 | 说明 |
|---------|------|
| `ANTHROPIC_AUTH_TOKEN` | 智谱 API Key |
| `ANTHROPIC_BASE_URL` | 智谱 API 端点 |
| `API_TIMEOUT_MS` | 请求超时时间（毫秒） |
| `CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC` | 禁用非必要流量 |

## 启动使用

```bash
# 进入项目目录
cd your-project

# 启动 Claude Code
claude
```

## claude code详细使用技巧

参考B站教程: https://www.bilibili.com/video/BV16GG5z9EDp/?spm_id_from=333.1391.0.0

视频中有详细的命令场景分析和实战教学

## 安装 Everything Claude Code 插件

Everything Claude Code (ECC) 是一套增强 Claude Code 的配置系统，包含 14 个专业代理、47 个领域技能、32 个斜杠命令和 9 种自动化钩子。

### 核心特性

- **让代码仓库自我教学** - 分析 git 历史，自动提取编码模式
- **持续学习** - 越用越智能，自动从会话中学习
- **专业代理分工** - TDD、代码审查、安全检查等各司其职
- **自动化钩子** - 自动格式化、类型检查、console.log 检测等

### 安装方式

在Claude Code中执行:

```bash
/plugin marketplace add affaan-m/everything-claude-code
```

然后在Claude Code中执行:

```bash
/plugin install everything-claude-code@everything-claude-code
```

### 基础使用步骤

装完以后，所有的命令、Agent、技能就都可以用了。开箱即用。

#### 第一步：项目计划
项目启动阶段新项目开始时，先别急着写代码。执行

```bash
/everything-claude-code:plan <你的实现计划>
```

让 Planner Agent 帮你把思路理清楚——需要什么功能、选什么技术栈、怎么分模块。

#### 第二步：开发过程
TDD 循环实际写代码的时候，用这个命令：

```bash
/everything-claude-code:tdd 开始编写代码
```

这会让 Claude 按照标准的 TDD 流程走：
- RED：先写测试，让它失败GREEN：写最少代码让测试通过
- REFACTOR：优化代码VERIFY：验证整个流程相比随意写代码，这种方式能显著降低 bug 率。而且如果后续需要改动，有测试作为保障，改起来心里才有底。

当完成了一个重要功能，使用：

```bash
/everything-claude-code:checkpoint
```

把当前的思路和状态快速记录下来。这既方便日后回滚，也能保留设计决策的思考轨迹。

#### 第三步：质量保障
不要跳过审查开发过程中常用：

```bash
/everything-claude-code:code-review 
```

让专门的 Review Agent 来审查你的代码。他们会检查：代码逻辑是否有漏洞安全隐患性能问题是否违反了规范

### 常用命令

| 命令 | 功能 |
|------|------|
| `/tdd` | 测试驱动开发 |
| `/code-review` | 代码质量审查 |
| `/plan` | 实现规划 |
| `/e2e` | 端到端测试 |
| `/build-fix` | 修复构建错误 |
| `/refactor-clean` | 重构清理 |
| `/verify` | 全面验证 |

## 相关资源

- [智谱AI官方文档](https://docs.bigmodel.cn/cn/coding-plan/quick-start)
- [智谱AI开放平台](https://open.bigmodel.cn/)
