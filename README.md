# 引文照妖镜 CiteMirror

给论文里的每一条参考文献验真：已证实存在 / 已证伪 / 元数据有误 / 无法核验，每条附证据。

纯前端单文件，不经过任何服务器；文献库：Crossref、OpenAlex。

判定规则：已证伪只有两种铁证（DOI 查无此号 / DOI 指向另一篇）；无 DOI 的文献永不判伪造；查不到 ≠ 是假的。

- 撤稿检测：读取 Crossref `updated-by`（Retraction Watch 数据），命中即标红
- 引文格式校验：按 GB/T 7714 常见要素粗判缺项
- 结果可导出 CSV / 打印为 PDF
