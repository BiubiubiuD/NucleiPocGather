# Nuclei Poc 全网收集
NucleiPocGather，每日更新

这个项目是一个 Python 脚本，用于批量克隆 GitHub 项目，获取 Nuclei POC，并将 POC 按类别分类存放到文件夹中。同时，使用 GitHub Action 每日自动运行脚本。
# POC 详情统计

> **当前项目 POC 更新时间：**`2026-08-13 13:42`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 106397 | cve | 60688 | medium | 43851 |
| 2 | wordpress | 99808 | other | 57149 | low | 37088 |
| 3 | wp-plugin | 91800 | wordpress | 5533 | high | 28738 |
| 4 | low | 34932 | sql | 5363 | info | 28079 |
| 5 | medium | 34620 | auth | 4237 | critical | 16502 |
| 6 | candidate | 34515 | remote_code_execution | 1992 | unknown | 130 |
| 7 | tech | 18928 | detect | 1867 | hight | 15 |
| 8 | detect | 18081 | web | 1415 | meduim | 11 |
| 9 | high | 17575 | microsoft | 1346 | informative | 5 |
| 10 | service | 13841 | default | 1215 | cretical | 4 |

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

