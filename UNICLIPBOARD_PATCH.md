# UniClipboard DNS 依赖修复

基线：n0-computer/n0-dns-resolver `16a791ce8cfd6456518970872ba3251b0756112d`（0.1.0）。

仅将 simple-dns 指向 UniClipboard/simple-dns 的不可变修复提交 `db89dd28485e890cc195ed8b1b1f6a78c5974a8e`；不修改解析器行为、网络设置和重试策略。完整 wire 回归由 simple-dns fork 维护。

上游发布包含 RFC 6891 OPT TTL 位字段修复的依赖后退出 fork。
