
# Sustech Adventure

**Sustech Adventure** 是一款基于 Unity 的 2D 校园互动叙事游戏。玩家扮演南科大学生，在考试前有限的 30 分钟内探索校园、完成任务、管理状态，并最终前往第三教学楼参加考试。

## 主要功能

- **多场景校园探索与世界地图** — 在宿舍、食堂、超市、图书馆、风雨操场等多个大场景和若干子场景自由移动，按 M 键打开手绘风格校园地图即可快速传送。
- **丰富 NPC 交互和场景交互** — 宿管阿姨、食堂阿姨、学长、学姐等 NPC 等你互动，包括 *对话*，*出示反应*，*支线任务*（现在主要是*兼职支线*）等多种交互方式；场景内的物品也可以点击交互。
- **两种过场动画和多种随机过场事件** — 过场时自动播报状态变更，移动途中随机触发校园生活小事件与支线任务。
- **实时状态 HUD 管理** — 时间、金钱、饱腹度、精神值实时显示，各属性互相制约，策略搭配是关键
- **背包与道具系统** — 背包界面查看已获得的物品，点击使用或出示。
- **商店与兼职的经济系统** — 在超市、贩卖机可以购买食物和复习资料；完成兼职任务赚取金钱。
- **多样小游戏** — 超市理货、记忆翻牌、图书馆排序、兼职配送、洗碗打工等 10+ 种网页小游戏。
- **多结局** — 失败有‘时间耗尽’，‘精神崩溃’，‘饥饿过度’等多种结局；考试结束根据成绩也有不同的结局，每个结局有相应的结局画面和文案。
- **快捷操作与进度保存** — M 键地图、B 键背包、Q 键快速保存、E 键快速读取，随时继续冒险。
- **Hint UI** — 会时刻对下一步行动提供提示，帮助玩家更好地理解游戏机制和目标。

### 操作说明

| 按键 | 功能 | 分类 |
|------|------|------|
| `M` | 打开/关闭世界地图 | 游戏 |
| `B` | 打开/关闭背包 | 游戏 |
| `Return` | 使用/出示选中道具 | 游戏 |
| `Ctrl` | 加速对话 | 游戏 |
| `Esc` | 关闭所有 UI，返回主镜头 | 系统 |
| `Q` | 快速存档 | 系统 |
| `E` | 快速读档 | 系统 |
| `S` | 小游戏直接胜利（调试用） | Debug |
| `F` | 小游戏直接失败（调试用） | Debug |


## 技术栈

| 技术 | 用途 |
|---|---|
| Unity 2022.3.62f3c1 | 游戏引擎 |
| C# | 游戏逻辑与编辑器扩展 |
| Ink + InkFungus | 分支叙事与对话系统 |
| Fungus | 对话流程可视化编排 |
| TextMesh Pro | UI 文字渲染 |
| SpriteGlow | 轮廓发光效果 |
| WebGL | 构建发布平台 |

## 安装与运行

### 从源码运行

1. 安装 [Unity Hub](https://unity.com/download) 和 Unity 2022.3.62f3c1
2. 安装 Git LFS：
   ```bash
   # Windows
   choco install git-lfs
   # macOS
   brew install git-lfs
   # Linux (Debian/Ubuntu)
   curl -s https://packagecloud.io/install/repositories/github/git-lfs/script.deb.sh | sudo bash
   sudo apt-get install git-lfs
   ```
3. 克隆仓库并初始化 LFS：
   ```bash
   git lfs install
   git clone https://github.com/sustech-cs304/team-project-26spring-26s-32.git
   ```
4. 在 Unity Hub 中打开 `unity/Sustech Adventure/` 目录
5. 在 `Scenes/Opening` 场景中点击 ▶ 运行
<img width="2144" height="1140" alt="862e4ee26f2a0f6d8eeecadec948da60" src="https://github.com/user-attachments/assets/36941371-e951-47b3-b140-3f739a2d9ca0" />
<img width="2129" height="1290" alt="9923158d7c79b00e85a8c75566ba847c" src="https://github.com/user-attachments/assets/1bde179a-37de-41e6-acfd-4a01701eda58" />
<img width="2129" height="1290" alt="2d7a11eb20ecc39bd4f9a7c52d58b77c" src="https://github.com/user-attachments/assets/5a614469-b5b3-4933-a40f-ca5520c681cd" />

### 直接游玩

访问以下链接即可在浏览器中游玩：  

- https://mkbk0614.itch.io/sustech
- https://sustech-adv.vercel.app
- https://play.unity.com/en/games/71bf287d-e7c2-431f-a634-08e7f9509119/sustech-adventure-game
> 注意：推荐使用 itch.io 版本，unity.com 版本可能不太稳定，而 vercel.app 版本是经过压缩的。

## 截图
开场画面
<img width="1065" height="525" alt="image" src="https://github.com/user-attachments/assets/99c410e5-d617-42d0-a6ab-090526844a7a" />

校园地图界面

<img width="822" height="456" alt="0f26951c16b2cdca64f49da5cb5dcdeb" src="https://github.com/user-attachments/assets/231a4696-43ed-4ec4-a490-96f0c7f8a9ee" />

对话与选择分支

<img width="1458" height="900" alt="5ca0fbe9caaf04c8f1899d486b19289f" src="https://github.com/user-attachments/assets/78b7fcb6-556b-4cb2-9ecc-0250cdc27dfe" />

小游戏界面

<img width="1152" height="1110" alt="b585a6cd6aa7cd39fbfd08433bed06e8" src="https://github.com/user-attachments/assets/26bd2616-bdbf-4001-a121-26a82589a00e" />

背包与道具系统

<img width="744" height="161" alt="a4cf0ba2f2548a6824d6fe3800bc9f4c" src="https://github.com/user-attachments/assets/f7d2e796-185e-4805-a30e-53643b0b4f0d" />

## 已知问题
- 部分情况下镜头容易被卡在聚焦情况，需要重置镜头（按 Esc 键）才能恢复正常
- 理智值的平衡性需要进一步调整
- Save & Load 功能中，目前 Load 的实现是动态地将人物重新投放到场景中，会重新触发一些事件（如进入场景的事件），导致一些不必要的副作用。
- 食堂被放到了 *风雨操场* 的位置，😄神了😄
- Unity WebGL 打包可能出现的问题：
![](https://p6-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/a28adb8b021446e7958c8768436c1315.png~tplv-a9rns2rl98-image.png?lk3s=8e244e95&rcl=2026052418035315A26A3C5F8B5ED99589&rrcfp=dafada99&x-expires=2095841034&x-signature=dvyx5yiLNGBbFJPDFxpduYnR3Yc%3D)
> 解决办法：
> - 打开 Unity → File → Build Settings → Player Settings
> - 找到 WebGL → Publishing Settings
> - 把 Compression Format 从 Brotli 改成 Disabled（或 Gzip）
> - 重新打包 WebGL，再用 Python 服务器打开，就不会有 .br 文件

## 相关链接

- [Ink 编剧指导](<version/2026.5.9 ink-program.md>)
- [InkFungus 入门教程](<version/2026.4.28 inkfungus-tutorial.md>)
- [项目 Wiki](https://github.com/sustech-cs304/team-project-26spring-26s-32/wiki)（如已启用）

## CI/CD

项目使用 GitHub Actions 自托管 Runner 进行持续集成：

- **触发条件**: push 到 `main` 分支
- **流水线步骤**:
  1. Checkout + LFS
  2. 运行 EditMode 测试
  3. 构建 WebGL 目标
- 配置文件: `.github/workflows/ci.yml`
