# Luckbit Wallet 隐私政策

语言：简体中文 | [English](privacy-policy.en.html) | [繁體中文](privacy-policy.zh-TW.html) | [日本語](privacy-policy.ja.html) | [한국어](privacy-policy.ko.html) | [Français](privacy-policy.fr.html) | [Español](privacy-policy.es.html) | [Русский](privacy-policy.ru.html) | [العربية](privacy-policy.ar.html)

最后更新：2026-01-31

本隐私政策适用于 Luckbit Wallet 浏览器扩展（以下简称“本扩展”）。本扩展为非托管钱包，私钥仅在本地加密保存，我们不托管、不接触用户私钥或资产。

## 1. 我们收集哪些信息
我们**不会收集、存储或出售**任何可识别用户身份的信息。  
本扩展不要求注册账号，也不需要登录即可使用核心功能。

## 2. 本地数据存储
为实现钱包功能，本扩展会在**用户本地设备**保存以下数据（仅本地存储，不上传）：
- 加密后的私钥/助记词
- 账户与网络配置
- 代币信息与交易记录缓存
- 用户设置（语言、自动锁定等）

所有敏感数据均在本地加密存储，扩展无法读取明文私钥或助记词。

## 3. 与第三方服务的通信
为完成链上查询与交易广播，本扩展需要与区块链节点/区块浏览器等第三方服务通信。这些请求可能包含：
- 钱包地址
- 交易哈希
- 网络与链 ID
- 用户设备的 IP 地址（由网络请求自然产生）

这些通信仅用于完成钱包功能，本扩展**不会**将用户数据共享或出售给第三方。

## 4. 权限说明（隐私相关）
- `storage` / `unlimitedStorage`：用于本地保存钱包数据与设置
- `tabs` / `activeTab`：用于与当前 DApp 页面交互、连接授权与打开必要页面
- `alarms`：用于自动锁定计时器
- `<all_urls>` 主机权限：用于在任意 DApp 页面注入 Provider 并完成授权流程

## 5. 数据安全
我们采用本地加密机制与自动锁定策略保护用户数据。请妥善保管您的助记词与密码，丢失后无法恢复。

## 6. 数据删除
用户可在扩展内“重置钱包”或清除浏览器扩展数据，以删除本地所有钱包信息。删除后无法恢复，请提前备份助记词。

## 7. 联系我们
如有隐私相关问题，请联系：  
邮箱：info@luckbit.link  
团队：luckbit  
隐私政策链接：https://victorlee2077.github.io/luckbit_docs/privacy-policy.html
