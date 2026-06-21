# Codex 测试

用本地 Codex CLI 批量测试一道糖果数学题，并统计 reasoning tokens 与正确率。

## 用法

该脚本无任何第三方依赖，只需要您已安装并登录 [Codex CLI](https://github.com/openai/codex)

```bash
python codex_candy_eval.py -m gpt-5.5 -r high -n 5
```

参数：

- `-m, --model`：codex 模型名，省略则用本地默认
- `-r, --reasoning-effort`：`low` / `medium` / `high` / `xhigh`（默认 `medium`）
- `-n, --tests`：测试次数（默认 1）

正确答案为 **21**，脚本直接判断回答中是否出现独立的 `21`。
