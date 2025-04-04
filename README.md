#原作者地址：https://github.com/qq254950134/my-iptv

homeTV 是一个用于个人托管和管理直播源的项目，旨在自动从多个网站获取最新的直播源，并对这些直播源进行整理、分类和去重处理。该项目适合用于个人学习、探索自动化脚本和 IPTV 直播源管理。 项目主页: 点击访问

直播源地址:https://cg.2539525949.xyz/final_streams.txt

## 功能介绍

- **自动获取直播源**：项目从多个指定的网站自动获取最新的直播源，支持 M3U 和 TXT 格式的源文件。
- **分类与整理**：自动根据节目名称对直播源进行分组整理，并对重复的源链接进行去重。
- **支持 IPv4 和 IPv6**：可以识别并分类不同类型的 IP 源地址，分为 IPv4 和 IPv6 进行整理。
- **输出格式**：抓取和整理后的直播源保存为 `final_streams.txt` 文件，方便进一步处理和使用。

## 项目结构

```bash
my-tv/
  ├── .github/
  │   └── workflows/
  │       └── schedule_run.yml  # 定时任务的 GitHub Actions 工作流
  ├── fetch_streams.py           # 主要的直播源抓取和整理脚本
  ├── final_streams.txt          # 保存抓取和整理后的直播源文件
  └── README.md                  # 项目介绍文件


```

## GitHub Actions 定时任务

项目已经配置了 GitHub Actions 工作流（`.github/workflows/schedule_run.yml`），它会每天 UTC 时间的 00:00 和 12:00 自动运行脚本抓取最新的直播源，并将结果推送到仓库。

### **法律声明**

<span style="color:red;">**此项目仅用于学习和研究目的。使用者在使用该项目时应遵守当地法律法规。请勿将此项目用于任何违反法律的活动。项目作者不对因使用此项目造成的任何法律问题负责。**</span>