<div align="center">

# 🔥 凤凰战机 Phoenix Fighter

**一款炫酷的街机风 Web 射击游戏 · 单文件 HTML5 Canvas**

![HTML5](https://img.shields.io/badge/HTML5-Canvas-orange)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)
![No Dependencies](https://img.shields.io/badge/Dependencies-0-green)
![License](https://img.shields.io/badge/License-MIT-blue)

霓虹战机 · 自动连射 · 连击加分 · Boss 挑战 · 粒子爆炸

</div>

---

## 🎮 在线游玩

克隆后直接用浏览器打开即可，无需任何构建 / 安装：

```bash
git clone https://github.com/Neonity2020/phoenix-fighter.git
cd phoenix-fighter
open index.html        # macOS
# 或
xdg-open index.html    # Linux
# 或
python3 -m http.server 8080
# 访问 http://localhost:8080
```

> 也可以开启 GitHub Pages 后在线游玩（见下方部署说明）。

---

## 🕹️ 操作说明

| 操作 | 键盘 | 触摸 / 鼠标 |
|------|------|-------------|
| 移动战机 | `W A S D` / `← ↑ ↓ →` | 拖动屏幕 |
| 射击 | **自动射击**（无需按键） | 自动射击 |
| 凤凰炸弹 | `B` | 拾取 `B` 道具自动释放 |
| 暂停 | `P` | - |
| 静音 | `M` | - |
| 全屏 | 双击屏幕 | 双击屏幕 |

---

## ✨ 游戏玩法

### 敌机类型

| 敌机 | 特点 | 分数 |
|------|------|------|
| 🩷 侦察机 | 速度适中，血量 1 | 100 |
| 💜 蛇形机 | 左右蛇形走位，血量 2 | 200 |
| 🧡 重装坦克 | 血量 5，会发射敌方子弹 | 400 |
| 🩵 速降机 | 极速俯冲，血量 1 | 150 |
| 👹 **BOSS 毁灭母舰** | 每关末尾出现，血条 + 弹幕攻击 | 5000 |

### 道具系统

击坠敌机有概率掉落道具，拾取生效：

| 道具 | 效果 |
|------|------|
| `P` 粉色 | 🔥 火力强化 Lv1 → Lv4（单发 → 双发 → 三叉 → 五路弹幕） |
| `S` 青色 | 🛡 能量护盾（抵挡一次伤害，最多叠 3 层） |
| `★` 金色 | ♥ 生命 +1（最多 5 条命） |
| `B` 绿色 | 💥 凤凰炸弹：全屏清弹 + 范围伤害 |

### 核心机制

- **自动射击**：战机全程自动连射，玩家专注走位
- **COMBO 连击**：连续击杀积累连击，分数倍增
- **关卡递进**：击坠 Boss 后进入下一关，敌机刷新更快、Boss 更强
- **最高分保存**：`localStorage` 持久化最高分
- **街机音效**：WebAudio 合成射击 / 爆炸 / 拾取音效，无需音频文件

---

## 🎨 特效

- ✨ 霓虹发光战机 + 引擎火焰 + 机翼倾斜
- 💥 粒子爆炸 · 屏幕震动 · 闪屏
- 🌌 滚动星空 + 星云背景
- 👹 Boss 血条警告 + 弹幕攻击

---

## 🛠️ 技术栈

单文件实现，零依赖：

```
phoenix-fighter/
└── index.html   # HTML + CSS + JS 全部内嵌
```

- **Canvas 2D** 渲染游戏画面（支持 DPR 高清屏）
- **requestAnimationFrame** 游戏循环 + `dt` 帧率无关
- **WebAudio API** 程序化合成音效
- **响应式布局** + 触摸事件，支持手机 / 平板 / 桌面

---

## 🚀 部署到 GitHub Pages

仓库 → Settings → Pages → Source 选择 `main` 分支根目录，保存后访问：

```
https://neonity2020.github.io/phoenix-fighter/
```

---

## 📁 项目结构

```
phoenix-fighter/
├── index.html    # 游戏本体（单文件）
├── README.md     # 本文档
└── .gitignore
```

---

## 🤝 参与贡献

欢迎提交 Issue / PR！可以尝试：

- 新增武器 / 僚机系统
- 新增 Boss 形态 / 弹幕模式
- 手柄支持、双人模式
- 优化性能与移动端手感

---

## 📄 License

MIT © Neonity2020

---

<div align="center">

⭐ 如果喜欢，欢迎 Star 支持！

**凤凰出击，星际无敌！🔥**

</div>
