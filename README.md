# 孙笑川桌宠 | Sun Xiaochuan Desktop Pet

一个使用 C# / WinForms 开发的 Windows 桌面宠物，配有孙笑川原版动图、照片和语音。支持独立多桌宠、鼠标互动、不同性格、带队巡游，以及多人开会。

A Windows desktop pet built with C# and WinForms, featuring Sun Xiaochuan’s original animations, photos, and voice clips. Includes independently configurable pets, mouse interactions, personalities, group parades, and lively meetings.
<img width="530" height="1130" alt="sxc2" src="https://github.com/user-attachments/assets/a163f14d-0cad-4ef0-88b1-ff64f8dd0ffc" />
<img width="2879" height="1526" alt="sxc01" src="https://github.com/user-attachments/assets/d70eaf2d-7be8-4462-badc-acb2b7e1c0b5" />
<img width="2879" height="1531" alt="sxc3" src="https://github.com/user-attachments/assets/f9e3abfc-bee8-4176-9f78-e9e0ffd2c201" />

---

## 中文说明

### 功能介绍

- **原声语音与语音盒**
  点击桌宠随机播放一句原声；可搜索台词、选择播放、调整音量或静音，也可以开启定时随机说话。启动时根据白天或夜晚播放对应问候。

- **桌面游走与鼠标互动**
  支持随机游走、调整移动速度，向右移动时自动镜像。桌宠偶尔会追逐鼠标，鼠标靠近时会稍微加速躲开。可以拖动位置、滚轮调整大小，也能暂停所有移动。

- **“下崽”与独立多桌宠**
  右键“下崽”即可生成另一只独立桌宠。每只拥有自己的位置、大小、音量、性格、说话间隔和随机计时；可以单独收起或删除，退出后保留剩余桌宠的档案。

- **名字与性格**
  默认按照创建顺序命名为“孙笑川一世、二世……”，支持自定义名字。提供好奇、胆小、暴躁、懒狗、话痨、闷葫芦六种性格，影响移动速度、鼠标互动倾向和自动说话频率。

- **偶发带队巡游**
  同一屏幕上的多只桌宠偶尔会自行组成队伍，跟随带队者走一圈。也可以手动发起、结束巡游，或设置某只不参加。

- **开会与集体发言**
  随机召集 2～12 只符合条件的同屏桌宠，到会场集合。支持“轮流发言”和允许声音重叠的“热闹讨论”，可调整人数、会议时长和发言间歇，也能随时散会。会议结束后恢复各自平时的行为和说话设置。

- **统一控制面板**
  在一个窗口中查看所有桌宠，按名字、编号或性格搜索，支持全选、反选和批量修改。可统一设置音量、大小、性格、说话间隔、移动行为等，也能批量显示、收起、静音、暂停或删除。只修改勾选的字段，保留其他个性化设置。

- **内置语音与便携运行**
  分享包中的语音封装在 `assets/voices.sxc`，通过相对路径读取。解压整个文件夹即可运行，也可以选择自己的外部语音目录。

- **其他便利功能**
  支持动图 / 照片切换、窗口置顶、托盘找回、多显示器移动，以及桌宠设置和位置保存。

> 语音来自预录音频，开会时也是随机播放原声，不是 AI 生成的实时对话。

### 使用方法

1. 在 Releases 中下载 **`SxcPet-share.zip`**。
2. **解压整个文件夹**，不要只取出 EXE。
3. 双击 **`SxcPet.exe`** 启动。
4. 右键桌宠或托盘图标，可打开语音盒、控制面板和开会设置。

常用操作：

| 操作 | 功能 |
| --- | --- |
| 左键点击 | 随机说一句 |
| 按住左键拖动 | 移动桌宠 |
| 鼠标滚轮 | 调整大小 |
| 右键 | 打开功能菜单 |
| 双击托盘图标 | 显示 / 找回桌宠 |

开会时，静音、收起、暂停移动、没有可用语音或正在忙碌的桌宠不会被召集。可以先通过控制面板统一调整状态。

### 系统要求

- Windows 10 / 11
- .NET Framework 4.8
- 无需安装 Python 或 Node.js，运行时无需联网

### 升级与分享

升级前退出旧版，将新版程序文件覆盖到原目录，并保留：

- `data`：桌宠档案和设置
- `assets/voices.sxc`：内置语音包

**`SxcPet-share.zip` 是包含语音的分享包；源码 / 更新包不包含原始语音素材。** 如果自行从源码构建，可使用 `AudioPackBuilder.exe` 制作内置语音包和分享 ZIP。

---

## English

### Features

- **Original voice clips and voice browser**  
  Click a pet to play a random clip, search clips by name, select a specific line, adjust volume, or mute it. Optional automatic speech uses randomized intervals. Startup greetings change between daytime and nighttime.

- **Wandering and mouse interactions**  
  Pets wander around the desktop at adjustable speeds and mirror their animation when moving right. They may follow the cursor or move away a little faster when it gets close. Drag to reposition, scroll to resize, or pause all movement.

- **Independent pets and cloning**  
  Use “下崽” to create another pet with independent settings and timers. Each pet has its own position, size, volume, personality, and speech schedule. Hide or delete pets individually; remaining pets are restored on the next launch.

- **Names and personalities**  
  Default names follow a numbered dynasty: “孙笑川一世, 二世, …”. Custom names are supported. Six personalities—Curious, Timid, Hotheaded, Lazy, Talkative, and Quiet—affect movement, mouse interactions, and automatic speech frequency.

- **Group parades**  
  Pets on the same monitor occasionally form a parade and follow a leader. Start or stop a parade manually, or opt individual pets out.

- **Meetings and group chatter**  
  Randomly gather 2–12 eligible pets on the same monitor. Choose turn-taking or overlapping chatter, and customize attendance, duration, and speech gaps. End the meeting at any time; participants then resume their usual behavior.

- **Central control panel and batch editing**  
  View every pet in one place, search by name, number, or personality, and select multiple pets. Batch-edit volume, size, personality, speech intervals, movement, and more. Only explicitly selected fields are changed. Bulk show, hide, mute, pause, and delete actions are also available.

- **Bundled audio and portable distribution**  
  The share package includes audio in `assets/voices.sxc`, loaded relative to the application folder. Extract the complete folder and run. External voice folders are also supported.

- **Everyday conveniences**  
  Switch between animation and photo modes, keep pets on top, recover them through tray icons, move them between monitors, and retain their settings across launches.

> Speech uses prerecorded clips. Meeting dialogue is randomly selected audio, not AI-generated conversation.

### Getting Started

1. Download **`SxcPet-share.zip`** from Releases.
2. **Extract the entire folder.**
3. Double-click **`SxcPet.exe`**.
4. Right-click a pet or its tray icon to access the voice browser, control panel, and meeting settings.

| Action | Result |
| --- | --- |
| Left-click | Play a random voice clip |
| Left-click and drag | Move the pet |
| Mouse wheel | Resize the pet |
| Right-click | Open the menu |
| Double-click tray icon | Show / recover the pet |

Muted, hidden, movement-paused, busy pets, and pets without available audio are excluded from meeting invitations.

The application interface is currently in Chinese.

### Requirements

- Windows 10 / 11
- .NET Framework 4.8
- No Python, Node.js, or internet connection required at runtime

### Updating and Sharing

Exit the previous version before replacing application files. Keep:

- `data` — pet profiles and settings
- `assets/voices.sxc` — bundled audio

**The share package includes audio; source / update packages do not include the original voice assets.** When building from source, use `AudioPackBuilder.exe` to create the audio pack and distributable ZIP.
