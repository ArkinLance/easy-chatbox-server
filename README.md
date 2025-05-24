# easy-chatbox-server

easy-chatbox-ui 对应的后端大模型管理服务，基于 Python FastAPI 和 WebSocket 实现，负责会话管理、多租户支持、模型路由和权限控制。

---

## 主要特性

- 基于 FastAPI 实现高性能异步 WebSocket 服务  
- 支持多模型接入（OpenAI、私有模型、本地部署模型）  
- 统一消息协议，支持流式输出，提升聊天交互体验  
- 支持多租户隔离和基于 Token 的权限认证  
- 会话持久化，支持断线重连和多设备同步  
- 易于扩展和集成，便于定制业务逻辑  

---

## 适用场景

- 需要统一管理和调度多种大模型服务  
- 支持高并发、多用户的实时对话场景  
- 需要基于身份和权限做多租户数据隔离  
- 需要实现会话状态管理与消息流控  

---

## 环境依赖

- Python 3.9+
- FastAPI
- uvicorn
- websockets
- redis (用于会话管理)
- pydantic

---

## 安装

```bash
git clone https://github.com/zkdtech/easy-chatbox-server.git
cd easy-chatbox-server
pip install -r requirements.txt