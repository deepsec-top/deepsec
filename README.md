# DeepSec 语料库

本仓库为 DeepSec 项目托管的开源中文网络安全运营语料库，包含原始语料文件、处理脚本和处理后的输出数据，旨在支持安全运营场景下的大模型训练。

## 目录结构

- `raw_corpus/`：原始YAML格式语料文件，按类别组织（如：漏洞响应、后门木马、钓鱼攻击、信息泄露）。
- `scripts/`：用于语料转换和验证的 Python 脚本。
- `dataset/`：处理后的最终 CSV/Excel 文件，供模型训练使用。
- `docs/`：贡献者指南和文档。

## 快速开始

1. 克隆仓库：`git clone https://github.com/deepsec-top/deepsec.git`
2. 阅读 `docs/corpus_guidelines.md` 了解贡献规则。
3. 按照 `docs/file_naming_convention.md` 中的命名规范，通过拉取请求提交语料数据。

参考示例[`raw_corpus/IL/il-001-github_sensitive_information_leakage.yaml`](raw_corpus/IL/il-001-github_sensitive_information_leakage.yaml)

## 语料类别

- 高级持续性威胁(`APT`)：高级持续性威胁事件
- 后门木马 (`BT`)：后门木马事件
- 云安全配置错误 (`CM`)：云平台服务配置错误事件
- 拒绝服务攻击 (`DDoS`)：分布式拒绝服务攻击事件
- 防御成功(`DS`)：防御成功的案例
- 钓鱼攻击 (`FA`)：钓鱼攻击及APT活动事件
- 黑客工具 (`HT`)：黑客工具使用事件
- 信息泄露 (`IL`)：信息泄露事件
- 内部威胁 (`IT`)：内部威胁与横向移动事件
- 挖矿木马 (`MC`)：挖矿木马事件
- 软件供应链 (`SC`)：软件供应链事件
- 漏洞利用 (`VR`)：漏洞利用事件
- Web攻击 (`WA`)：Web攻击事件
- 持续补充优化中...
  

## 许可证

MIT 许可证，详见 [`LICENSE`](LICENSE) 文件。

## 联系方式

邮箱：admin@deepsec.top  
网站：[DeepSec 官网](https://deepsec.top)
加入社区：[DeepSec 社区](#)