# 发布检查记录

日期：2026-09-06。

## 已执行

- 使用 skill-creator 的 quick_validate.py 校验：通过 name/description 元数据、名称格式及入口脚手架检查。
- 检查 Markdown 相对文件链接：14 个均解析到本仓库内存在的文件。
- 解析 agents/openai.yaml 并核对默认调用名称：通过。
- 检查执行入口与参考文件：不使用原专业词表、私人全局路径或强制外部技能调用。
- 在 Windows 下用 ReportLab 生成两页自有合成 PDF，运行 pdfinfo 检查页数，再用 pdftotext -layout 提取：两页内容与分页位置核对通过。该测试仅验证示例读取路径，不代表对复杂排版或扫描图表的全面验证。

## 尚未执行

- 真实论文的端到端智能体阅读或评审测试。
- [回归场景](README.md) 的独立模型行为测试及人工专业验收。
- 视觉图表解析和 OCR 的环境兼容性矩阵测试。
- 不同学科的专业准确率测量、普通提示对照实验。
- ScienceHub 官方 research-skill-evaluator 评分。

本次通过的是发布结构检查与基础 PDF 工具检查。上述未执行项不得宣传成已通过或获得分数。
