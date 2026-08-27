# Surge Custom Rules

个人维护的 Surge 自定义规则。iPhone 安装一次远程 Module 后，后续更新继续使用同一个 URL。

## iOS 自定义规则

- Module：[`modules/ios-custom-rules.sgmodule`](modules/ios-custom-rules.sgmodule)
- 远程 URL：

  ```text
  https://raw.githubusercontent.com/anjieyang/surge-custom-rules/main/modules/ios-custom-rules.sgmodule
  ```

在 Surge 的 Module 页面选择从 URL 安装，并启用“自定义规则（iOS）”。

高德地图的开屏广告规则需要 Surge 的 MITM 功能，并信任 Surge CA 证书；解密范围仅包含 `m5.amap.com`。

模块同时使用系统 DNS、阿里 DNS 和 Cloudflare DNS，并关闭 Surge 的 IPv6 解析与 IPv6 VIF，以减少 iOS 在网络切换后显示已连接但无法联网的情况。

## 维护约定

- `modules/` 存放 Surge Module。
- 以后需要指定代理策略组的规则时，再增加 `rulesets/`。
- 不在公开仓库中保存节点、订阅地址、令牌或其他凭据。
