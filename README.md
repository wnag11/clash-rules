# clash-rules

Custom Clash/Mihomo rule-provider payloads for OpenClash.

## Raw rule URLs

```yaml
custom-x:
  type: http
  behavior: classical
  path: ./ruleset/custom-x.yaml
  url: https://raw.githubusercontent.com/wnag11/clash-rules/main/rules/X.yaml
  interval: 86400

finance-pay:
  type: http
  behavior: classical
  path: ./ruleset/finance-pay.yaml
  url: https://raw.githubusercontent.com/wnag11/clash-rules/main/rules/Finance-Pay.yaml
  interval: 86400

finance-info:
  type: http
  behavior: classical
  path: ./ruleset/finance-info.yaml
  url: https://raw.githubusercontent.com/wnag11/clash-rules/main/rules/Finance-Info.yaml
  interval: 86400

cloud-services:
  type: http
  behavior: classical
  path: ./ruleset/cloud-services.yaml
  url: https://raw.githubusercontent.com/wnag11/clash-rules/main/rules/Cloud.yaml
  interval: 86400
```

## Suggested policy mapping

```yaml
rules:
  - RULE-SET,custom-x,🐦 X服务
  - RULE-SET,finance-pay,💳 金融支付
  - RULE-SET,finance-info,📈 金融资讯
  - RULE-SET,cloud-services,☁️ 云服务
```
