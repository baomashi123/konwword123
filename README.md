# konwword123 — 小学→中学→高中背单词 Starter Repo

这是一个起始仓库样例，用于构建面向中国中小学（含中考/高考）背单词的 Web + 移动 App，支持离线学习、SRS(SM-2) 调度、教师/学生基础数据模型和词库导入。

快速开始

1. 本地运行后端：
   cd server
   npm install
   npm run seed
   npm start

2. 本地运行 Web 前端：
   cd client-web
   npm install
   npm run dev

3. (可选) 使用 Docker：
   docker-compose up --build

包含内容概要：
- server/: Express + SQLite 后端，包含 /api/words 和 /api/review 接口
- client-web/: React + Vite 前端，带 Service Worker 与 IndexedDB 离线示例
- shared/srs/sm2.js: SM-2 算法实现
- data/words.csv: 示例词表

如果你想我把更多功能（教师端、导入工具、React Native 演示）补上，我可以继续按优先级逐步提交。