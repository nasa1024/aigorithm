# AIGorithm：使用 Codex CLI 与 VS Code 的算法练习仓库

English version: see `README.md`.

本仓库面向使用 VS Code 与 Codex CLI 的“单题驱动”算法练习：由 Codex 出题与搭建模板，你完成实现与测试，之后 Codex 给出系统化评价与改进建议。

## 概览
- 目标：在 Codex CLI 的辅助下，用 Go 与 Python 进行算法练习。
- 流程：你提出学习需求 → Codex 出题并脚手架搭建 → 你实现 → 本地运行测试 → 通知 Codex 评价 → Codex 生成反馈与 `doc.md`。
- 范围：排序、查找、数据结构、递归、贪心、动态规划、图论、树结构等。

## 仓库结构
- `golang/` — Go 按类别组织（如 `sorting/`、`searching/`、`dp/`）。
- `python/` — Python 按相同方式组织。
- `templates/` — 各语言的题目模板，用于新题目脚手架。
- `solutions/` — 参考实现与最佳实践。
- `docs/` — 学习文档与算法分析、评价结果。

## 语言索引
- JavaScript/TypeScript：`javascript/`、`typescript/` — 使用 `node`/`ts-node` 运行，`npm test`（Jest/Mocha/Vitest）测试。
- Java：`java/` — 使用 Maven `mvn test` 或 Gradle `./gradlew test`。
- C++：`cpp/` — 使用 `g++` 或 CMake 构建；可用 `ctest` 测试。
- Rust：`rust/` — 使用 `cargo run` / `cargo test`。
- C#（.NET）：`csharp/` — 使用 `dotnet run` / `dotnet test`。
- 各语言的命令、风格与测试规范详见 `AGENTS.md`。

## 在 VS Code + Codex 中使用
- 在 VS Code 中打开本仓库。
- 在集成终端与 Codex 交互：表达想学的主题/难度，请求 Codex 搭建题目框架。
- Codex 会创建目录、模板与测试；你在模板中完成核心实现。
- 在本地运行测试并根据结果迭代；需要时向 Codex 请求提示或调试建议。
- 完成后通知 Codex 评价，Codex 输出评估与优化建议（如写入 `docs/<topic>/doc.md`）。


## 一次一道题的学习流程
1) 告诉 Codex 本次想练习的题目类型/难度；
2) Codex 按规范在 `golang/<类别>/<题目>/` 或 `python/<类别>/<题目>/` 搭建模板与测试；
3) 你在模板中完成核心逻辑；
4) 在题目目录运行测试并修正；
5) 通知 Codex 进行评价，Codex 生成 `doc.md` 与优化建议。

示例（Go：冒泡排序）：
- 路径：`golang/sorting/bubble_sort/`
- 在 `bubble_sort.go` 实现 `bubbleSort(nums []int) []int`，在该目录执行 `go test -v`。

## 说明
- 本仓库遵循 `AGENTS.md` 中的结构、编码/测试规范与评价流程。
- 可根据需要对 Go 使用 `gofmt`，对 Python 使用 `black/autopep8` 进行格式化。
- 使用有意义的命名，并在有助理解时添加简明注释。
