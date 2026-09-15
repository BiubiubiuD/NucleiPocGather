# Nuclei Poc 全网收集
NucleiPocGather，每日更新

这个项目是一个 Python 脚本，用于批量克隆 GitHub 项目，获取 Nuclei POC，并将 POC 按类别分类存放到文件夹中。同时，使用 GitHub Action 每日自动运行脚本。
# POC 详情统计

> **当前项目 POC 更新时间：**`2026-09-15 16:47`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 84525 | other | 56751 | medium | 35638 |
| 2 | wordpress | 77998 | cve | 41275 | low | 28825 |
| 3 | wp-plugin | 71904 | wordpress | 6851 | info | 27024 |
| 4 | candidate | 31770 | sql | 4631 | high | 26151 |
| 5 | low | 26485 | auth | 4089 | critical | 14271 |
| 6 | medium | 26388 | detect | 2473 | unknown | 136 |
| 7 | tech | 17491 | microsoft | 2017 | meduim | 19 |
| 8 | detect | 16665 | remote_code_execution | 1562 | informative | 17 |
| 9 | high | 14762 | api | 1123 | hight | 15 |
| 10 | service | 13834 | web | 1002 | cretical | 4 |

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

