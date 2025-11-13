# anything-llm

本專案用於在本地端透過 **Docker** 快速部署 **AnythingLLM**，並與本地的 **Ollama** 模型（如 `gemma3:1b`）進行串接。  
適合用於本地知識庫、文件搜尋、AI 助理等用途，所有資料皆留在本地端，隱私安全。

---

## 🚀 功能特點

- 一鍵啟動 AnythingLLM（透過 Docker Compose）
- 支援本地 LLM（使用 Ollama）
- 支援 Gemma、Llama、Qwen 等本地模型
- 文件上傳 → 建立知識庫 → 與文件進行 AI 對話
- 全程離線運作（取決於你的模型）

---

## 📦 前置需求

請先安裝以下工具：

- **Docker**
- **Docker Compose**
- **Ollama**（本地 LLM 執行框架）
- 至少一個模型，例如：

```bash
ollama pull gemma3:1b
```

## 🔧 安裝與啟動

```
git clone git@github.com:jasonjason1018/anything-llm.git
cd anything-llm/anythingllm
touch .env
cd ..
docker compose up -d
```
啟動後開啟:

👉 http://localhost:3001

## 🐳 停止服務
```
docker compose down
```