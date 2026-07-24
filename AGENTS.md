# FengGao Lab Runtime Data

本仓只承载 `fenggaolab.org` 可公开读取的运行时 JSON 投影；它不是 dashboard、认证状态或网站源码的 owner。

- `runtime/lab-ai-telemetry.json` 只能由授权的 telemetry automation 从 fresh dashboard session 生成；不得手工填写、猜测或复制旧数字。
- 禁止提交 token、cookie、浏览器 auth state、账户信息、原始响应或其他私有运行数据。
- 同步提交只应包含预期 runtime JSON；公开 currentness 必须由生成 receipt、仓库 bytes 和网站消费端 readback共同证明。
- 修改后至少运行 JSON 解析、`git diff --check` 和生成器定义的 schema/字段验证。

<!-- CODEGRAPH_START -->
## CodeGraph

- 本仓库使用本地 `.codegraph/` 索引；该目录不得纳入 Git。
- 定义、调用、影响范围和代码路径等结构检索优先使用 CodeGraph；字面文本检索使用 `rg`。
- 索引缺失或过期时运行 `codegraph init .` 或 `codegraph sync .`。
<!-- CODEGRAPH_END -->
