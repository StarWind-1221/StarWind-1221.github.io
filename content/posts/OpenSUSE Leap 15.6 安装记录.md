---
title: OpenSUSE Leap 15.6 安装记录
date: 2026-09-27
categories: Linux 折腾记录
---

<!--more--> 


## 一、系统更新
无需换源
```bash
sudo zypper update         # 通用包更新
```

---

## 二、安装 RIME 输入法（fcitx5-rime）
```bash
sudo zypper install fcitx5 fcitx5-rime fcitx5-gtk fcitx5-qt fcitx5-configtool librime*
```
**简体输出：** RIME 输入状态下按`` Ctrl+` `` 切换方案，选带“简化字”的。

---

## 三、中文字体
```bash
sudo zypper install google-noto-sans-cjk-fonts
sudo fc-cache -fv
```
然后重启或注销。

---

## 四、时区 / 时间问题
时区设为上海但慢 8 小时，是硬件时钟（RTC）解读方式不一致。解决：
```bash
sudo timedatectl set-local-rtc 1 --adjust-system-clock
```
然后开启 NTP 同步：
```bash
sudo timedatectl set-ntp true
```

---

## 五、终端（等宽）字体推荐

**YaHei Consolas Hybrid** —— Consolas + 微软雅黑缝合，民间合成字体，手动下载
**安装步骤：**
```bash
mkdir -p ~/.local/share/fonts
cp /path/to/font/*.ttf ~/.local/share/fonts/
fc-cache -fv
```
然后在 Konsole **设置 → 编辑当前方案 → 外观** 里选择该字体。