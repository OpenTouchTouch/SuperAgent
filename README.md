# 运行
```
# 配置模型key
cp env.example .env

#启动后端api
python main_api.py

# 进行测试
python a2a_client.py

# 查看每个Agent使用的模型
slide_agent/config.py

1.启动前端程序
cd AIReviewer/frontendSlide  

# 按照依赖
cp env_template .env 

##### npm install -g pnpm

pnpm install

# 设置数据库
pnpm db:push

# 启动开发服务器
pnpm dev


2.启动大纲生成程序
cd AIReviewer/slidegenerate/slide_outline

# 检查.env文件
 cp .env.example .env 

# 启动服务
 python main_api.py  

# 指定大模型启动服务
python main_api.py --provider deepseek --model deepseek-chat 


3.启动内容生成程序
cd AIReviewer/slidegenerate/slide_agent

# 检查.env文件
cp env.example .env

# 启动服务
 python main_api.py  

4.启动MCP查询智能体工具
cd AIReviewer/slidegenerate/slide_outline

# 启动转发

fastmcp run --transport sse --port 6501 mcpserver/rag_tool.py

5.启动MCP翻译智能体工具
cd AIReviewer/slidegenerate/slide_outline

fastmcp run --transport sse --port 6502 mcpserver/translate_tool.py

6.启动缓存程序
cd AIReviewer/example

python LLM_cache.py --provider deepseek --model deepseek-chat

7.执行代理报错

cd AlReviewer/slidegenerate/slide_outline

HTTP_PROXY=http://127.0.0.1:7890
HTTPS_PROXY=http://127.0.0.1:7890


```
