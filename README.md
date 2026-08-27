# Surge Custom Rules

个人维护的 Surge 自定义规则。iPhone 安装一次远程 Module 后，后续更新继续使用同一个 URL。

## iOS 自定义规则

- Module：[`modules/ios-custom-rules.sgmodule`](modules/ios-custom-rules.sgmodule)
- 远程 URL：

  ```text
  https://raw.githubusercontent.com/anjieyang/surge-custom-rules/main/modules/ios-custom-rules.sgmodule
  ```

在 Surge 的 Module 页面选择从 URL 安装，并启用“自定义规则（iOS）”。

## 维护约定

- `modules/` 存放 Surge Module。
- 以后需要指定代理策略组的规则时，再增加 `rulesets/`。
- 不在公开仓库中保存节点、订阅地址、令牌或其他凭据。
