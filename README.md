# Dler-Rules

个人代理规则集合，支持多种代理客户端配置格式。

## 支持的客户端

| 目录 | 客户端 |
|------|--------|
| `Clash/` | Clash / Mihomo |
| `Surge/` | Surge 2 / 3 / 4 |
| `QuantumultX/` | Quantumult X |
| `Quantumult/` | Quantumult |
| `Shadowrocket/` | Shadowrocket |
| `sing-box/` | sing-box |
| `Surfboard/` | Surfboard |
| `Auto/` | 自动选择规则 |
| `Profile/` | 配置文件模板 |

## 目录结构

```
Dler-Rules/
├── Clash/
│   ├── Head.yaml           # 基础头部配置
│   ├── Head_dns.yaml       # DNS 配置头
│   ├── Head_tap.yaml       # TAP 模式头
│   ├── Head_tun.yaml       # TUN 模式头
│   ├── Rule.yaml           # 规则集
│   └── Provider/           # 规则提供者
├── Surge/
│   ├── Cert.conf           # 证书配置
│   ├── Groups.conf         # 策略组
│   ├── MITM.conf           # MITM 配置
│   ├── Prototype.conf      # 原型配置
│   ├── Surge 2/
│   ├── Surge 3/
│   └── Surge 4/
├── QuantumultX/
├── Quantumult/
├── Shadowrocket/
├── sing-box/
├── Surfboard/
├── Auto/
├── Profile/
├── SSEncrypt.module        # Surge 加密模块
├── alibaba-https.mobileconfig    # 阿里巴巴 HTTPS 证书
├── cloudflare-https.mobileconfig # Cloudflare HTTPS 证书
├── dnspod-https.mobileconfig     # DNSPod HTTPS 证书
└── google-https.mobileconfig     # Google HTTPS 证书
```

## 使用方式

根据你使用的代理客户端，引用对应目录下的规则文件。各客户端通常支持远程规则订阅，将对应文件的 raw URL 填入订阅地址即可。

## 注意

这是个人私用规则集，不定期更新，无法保证对所有网络环境适用。
