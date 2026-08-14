# cali 的 Loon 分流配置

基于 iKeLee 的 Loon 进阶配置 + blackmatrix7/ios_rule_script 规则源。

## 使用方式

在 Loon 里「设置」→「高级」→「配置文件」→「导入远程配置文件」，粘贴：

```
https://raw.githubusercontent.com/febfengt/loon-config/main/config/loon.lcf
```

## 策略组

| 组 | 说明 |
|---|---|
| 香港/台湾/日本/韩国/新国/美国 手动/自动策略 | 按地区/场景分流 |
| 兜底后备策略 | 未匹配流量走这里 |

## 节点来源

- 机场1 / 机场2 / vps(白丝云)

## 规则来源

blackmatrix7/ios_rule_script（ShuntRules 同源数据）

## 首次使用

1. 导入远程配置文件：`https://raw.githubusercontent.com/febfengt/loon-config/main/config/loon.lcf`
2. 手动添加订阅节点（**不要**放在配置文件里）：
   - 设置 → 远程代理 → 添加
   - 名称填：`机场1` / `机场2` / `vps`
   - URL 粘贴各自的订阅链接
