# Course Inquiry Modern

- `apps/api/` 负责 FastAPI 接口、PKU 在线查询、离线 CSV 导入和 SQLite 索引。数据同步和建索引脚本在 `apps/api/scripts/`。
- `apps/web/` 是 React + Vite 前端，统一通过 API 查询和导出课程。离线默认使用仓库样例，完整上游 CSV 按 [README](README.md) 同步。
- 从项目根运行 `make api`、`make web`。涉及后端时运行 `make test`，涉及前端时运行 `npm --prefix apps/web run build`。
