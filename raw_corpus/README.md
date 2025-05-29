# DeepSec 网络安全运营语料库

## 📊 语料统计

| 分类 | 数量 | 说明 |
|------|------|------|
| 后门木马 (BT) | 3 | 包含CobaltStrike、冰蝎等后门木马检测案例 |
| 黑客工具 (HT) | 4 | 包含各类渗透测试和攻击工具检测案例 |
| Web攻击 (WA) | 4 | 包含SQL注入、模板注入、反序列化等Web攻击案例 |
| 挖矿相关 (MC) | 1 | 包含挖矿木马通信检测案例 |
| 漏洞利用 (VR) | 1 | 包含Exchange ProxyLogon等漏洞利用案例 |
| 信息泄露 (IL) | 2 | 包含GitHub敏感信息泄露、Web目录遍历等案例 |
| 钓鱼攻击 (FA) | 0 | 暂无语料 |

**总计：15个语料文件**

---

## 📁 语料详细列表

### 🔴 后门木马 (BT - Backdoor Trojan)

| ID | 语料标题 | 贡献人 |
|----|----------|--------|
| bt-003 | [后门木马-webshell-上传内存马通信](BT/bt-003-webshell_upload_memory_shell.yaml) | FOOL |
| bt-004 | [后门木马-CobaltStrike Beacon HTTP上线](BT/bt-004-cobaltstrike_beacon_http.yaml) | FOOL |
| bt-005 | [后门木马-冰蝎4.0 PHP Webshell通信](BT/bt-005-webshell_behinder_4_0.yaml) | FOOL |

### 🔧 黑客工具 (HT - Hacker Tool)

| ID | 语料标题 | 贡献人 |
|----|----------|--------|
| ht-002 | [黑客工具-SMBExec远程执行工具](HT/ht-002-smbexec_remote_execution.yaml) | FOOL |
| ht-003 | [黑客工具-毒刺pystinger隧道通信](HT/ht-003-pystinger_tunnel_communication.yaml) | FOOL |
| ht-004 | [黑客工具-Metasploit远控Payload传输](HT/ht-004-metasploit_payload_transmission.yaml) | FOOL |
| ht-005 | [黑客工具-neo-reGeorg加密隧道通信](HT/ht-005-neo_regeorg_tunnel_communication.yaml) | FOOL |

### 🌐 Web攻击 (WA - Web Attack)

| ID | 语料标题 | 贡献人 |
|----|----------|--------|
| wa-001 | [Web攻击-SQL注入攻击](WA/wa-001-sql_injection_attack.yaml) | FOOL |
| wa-002 | [Web攻击-Java FreeMarker模板注入](WA/wa-002-freemarker_template_injection.yaml) | FOOL |
| wa-003 | [Web攻击-Python反序列化漏洞](WA/wa-003-python_unpickle_deserialization.yaml) | FOOL |
| wa-004 | [Web攻击-反弹shell攻击](WA/wa-004-reverse_shell_attack.yaml) | FOOL |

### ⛏️ 挖矿相关 (MC - Mining/Cryptocurrency)

| ID | 语料标题 | 贡献人 |
|----|----------|--------|
| mc-001 | [挖矿木马-挖矿木马外联通信](MC/mc-001-mining_trojan_communication.yaml) | FOOL |

### 🔓 漏洞利用 (VR - Vulnerability Response)

| ID | 语料标题 | 贡献人 |
|----|----------|--------|
| vr-001 | [漏洞利用-Exchange ProxyLogon远程代码执行](VR/vr-001-exchange_proxylogon_cve_2021_27065.yaml) | FOOL |

### 📋 信息泄露 (IL - Information Leakage)

| ID | 语料标题 | 贡献人 |
|----|----------|--------|
| il-001 | [信息泄露-github敏感信息泄露](IL/il-001-github_sensitive_information_leakage.yaml) | [@deepsec-top](https://github.com/deepsec-top) |
| il-002 | [Web根目录文件遍历导致信息泄露，可下载/etc/passwd文件](IL/IL-002-web_root_directory_information_leakage.yaml) | [@wzfukui](https://github.com/wzfukui) |

### 🎣 钓鱼攻击 (FA - Fishing Attack)

| ID | 语料标题 | 贡献人 |
|----|----------|--------|
| - | 暂无语料 | - |

---

## 📝 语料格式说明

每个语料文件都包含以下标准化字段：

- **ID**: 唯一标识符（格式：类别前缀-序号）
- **Category**: 语料分类
- **Created_At**: 创建时间
- **Contributors**: 贡献者列表
- **Additional_Info**: 附加信息
- **Title_CN**: 中文标题
- **Title_EN**: 英文标题
- **Question**: 安全事件场景描述
- **Complex_CoT**: 复杂思维链推理过程
- **Response**: 具体响应措施
- **Log_Sample**: 相关日志样本

## 🔗 相关链接

- [项目主页](../README.md)
- [贡献指南](../docs/CONTRIBUTING.md)
- [原始语料目录]()
- [处理脚本目录](../scripts/)

---

## 👥 贡献者

感谢以下贡献者为本项目提供的语料：

- **FOOL** - 主要贡献者，提供了大部分安全检测语料
- **[@deepsec-top](https://github.com/deepsec-top)** - 提供GitHub信息泄露和SMBExec工具检测语料
- **[@wzfukui](https://github.com/wzfukui)** - 提供Web目录遍历信息泄露语料

*最后更新时间：2025-05-29* 