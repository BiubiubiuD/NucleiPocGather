# Nuclei Poc 全网收集
NucleiPocGather，每日更新

这个项目是一个 Python 脚本，用于批量克隆 GitHub 项目，获取 Nuclei POC，并将 POC 按类别分类存放到文件夹中。同时，使用 GitHub Action 每日自动运行脚本。
# POC 详情统计

> **当前项目 POC 更新时间：**`2026-08-27 22:20`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 96654 | other | 56228 | medium | 40274 |
| 2 | wordpress | 90168 | cve | 50278 | low | 34029 |
| 3 | wp-plugin | 83462 | sql | 9134 | high | 28155 |
| 4 | candidate | 32462 | wordpress | 5975 | info | 27511 |
| 5 | low | 31571 | auth | 4596 | critical | 15100 |
| 6 | medium | 30797 | remote_code_execution | 3918 | unknown | 139 |
| 7 | tech | 17553 | detect | 1972 | informative | 17 |
| 8 | detect | 16657 | web | 1445 | hight | 15 |
| 9 | high | 16546 | microsoft | 1294 | meduim | 9 |
| 10 | service | 13833 | api | 1145 | cretical | 4 |

**81 个目录，44572 个文件**
## 如何使用

### 克隆项目

克隆这个项目到本地：

```bash
git clone https://github.com/lianqingsec/NucleiPocGather.git
```

进入项目目录：

```bash
cd NucleiPocGather
```

### 配置

在 `repo.txt` 文件中配置监控 GitHub 项目信息。

### 运行脚本

运行 Python 脚本：

```bash
python NucleiPocGather.py
```

### GitHub Action

在 GitHub 仓库中设置 Action，以便每日自动运行脚本。

> 需要配置`Workflow permissions`为`Read and write`权限

## 文件结构

- `NucleiPocGather.py`: 收集全网 Nuclei POC 的脚本文件。
- `DeWeight.py`: 对现有的 Nuclei POC 进行进一步去重的脚本文件。
- `WirteREADME.py`: 统计现有的 POC 并更新 README.md 文件。
- `repo.txt`: Nuclei POC 仓库列表。
- `poc.txt`: 已存档 POC 列表。
- `poc/`: 存放分类后的 Nuclei POC 文件夹。

