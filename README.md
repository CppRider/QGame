# QGame开发文档

## [click here](./.manual/en/quickstart.md) to visit the doc_en.

> QGame意为Quick Game或Cute Game，是一个基于[SDL](http://www.libsdl.org/)及其附加库开发的轻量级跨平台Lua游戏库，开发者可以通过简单的Lua脚本制作出效率和体积都十分出色的游戏程序，目前版本的QGame可以提供图像渲染、媒体播放控制，以及系统信息的获取和完善的交互事件处理等功能，如果在使用过程中出现任何问题或有任何建议，请开个issue。

## 1. API字母顺序总览

详情参见此处 [APIList](./.manual/zh/APIList.md)

## 2. API功能分类及介绍

### 2.1 QGame库基础功能

详情参见此处 [Basic.md](./.manual/zh/Basic.md)

### 2.2 QGame库窗口操作

详情参见此处 [Window.md](./.manual/zh/Window.md)

### 2.3 QGame库图形相关操作

详情参见此处 [Graphic.md](./.manual/zh/Graphic.md)

### 2.4 QGame库媒体相关操作

详情参见此处 [Media.md](./.manual/zh/Media.md)

### 2.5 QGame库交互事件处理

详情参见此处 [Action.md](./.manual/zh/Action.md)

### 2.6 QGame库其它功能

详情参见此处 [Others.md](./.manual/zh/Others.md)

## 3. 附录

> ## 键盘事件对应表

### ***前缀***

| 值        | 描述     |
|:----------|:---------|
| "KEYDOWN" | 按键按下 |
| "KEYUP"   | 按键抬起 |

### ***后缀***

**注意：**
部分字符的按键事件为虚拟事件，在大部分键盘上可能无法通过物理按键触发

| 值              | 描述            |
|:----------------|:----------------|
| "0"             | 0               |
| "00"            | 00              |
| "000"           | 000             |
| "1"             | 1               |
| "2"             | 2               |
| "3"             | 3               |
| "4"             | 4               |
| "5"             | 5               |
| "6"             | 6               |
| "7"             | 7               |
| "8"             | 8               |
| "9"             | 9               |
| "F1"            | F1              |
| "F2"            | F2              |
| "F3"            | F3              |
| "F4"            | F4              |
| "F5"            | F5              |
| "F6"            | F6              |
| "F7"            | F7              |
| "F8"            | F8              |
| "F9"            | F9              |
| "F10"           | F10             |
| "F11"           | F11             |
| "F12"           | F12             |
| "F13"           | F13             |
| "F14"           | F14             |
| "F15"           | F15             |
| "F16"           | F16             |
| "F17"           | F17             |
| "F18"           | F18             |
| "F19"           | F19             |
| "F20"           | F20             |
| "F21"           | F21             |
| "F22"           | F22             |
| "F23"           | F23             |
| "F24"           | F24             |
| "A"             | A               |
| "B"             | B               |
| "C"             | C               |
| "D"             | D               |
| "E"             | E               |
| "F"             | F               |
| "G"             | G               |
| "H"             | H               |
| "I"             | I               |
| "J"             | J               |
| "K"             | K               |
| "L"             | L               |
| "M"             | M               |
| "N"             | N               |
| "O"             | O               |
| "P"             | P               |
| "Q"             | Q               |
| "R"             | R               |
| "S"             | S               |
| "T"             | T               |
| "U"             | U               |
| "V"             | V               |
| "W"             | W               |
| "X"             | X               |
| "Y"             | Y               |
| "Z"             | Z               |
| "ESC"           | Esc             |
| "ENTER"         | Enter           |
| "BACKSPACE"     | Backspace       |
| "UP"            | ↑               |
| "DOWN"          | ↓               |
| "LEFT"          | ←               |
| "RIGHT"         | →               |
| "INSERT" | Insert |
| "DELETE" | Delete |
| "HOME" | Home |
| "END" | End |
| "PAGEUP" | PageUp |
| "PAGEDOWN" | pageDown |
| "LCTRL" | 左Ctrl键 |
| "LGUI" | 左GUI键（Windows系统下为Win键，Mac系统下为Command键） |
| "LALT" | 左Alt键 |
| "LSHIFT" | 左Shift键 |
| "RCTRL" | 右Ctrl键 |
| "RGUI" | 右GUI键（Windows系统下为Win键，Mac系统下为Command键） |
| "RALT" | 右Alt键 |
| "RSHIFT" | 右Shift键 |
| "SPACE" | 空格键 |
| "TAB" | Tab键 |
| "CAPSLOCK" | CapsLock |
| "NUMLOCK" | NumLock |
| "PRINTSCREEN" | PrintScreen |
| "SCROLLLOCK" | ScrollLock |
| "PAUSE" | 媒体播放暂停键 |
| "AUDIOMUTE" | 静音键 |
| "AUDIOPREV" | 媒体播放上一首键 |
| "AUDIONEXT" | 媒体播放下一首键 |
| "AUDIOPLAY" | 媒体播放开始键 |
| "AUDIOSTOP" | 媒体播放停止键 |
| "VOLUMEUP" | 音量增大键 |
| "VOLUMEDOWN" | 音量减小键 |
| "BRIGHTNESSUP" | 亮度增加键 |
| "BRIGHTNESSDOWN" | 亮度减少键 |
| "BACKQUOTE" | ` |
| "EXCLAM" | ! |
| "AT" | @ |
| "HASH" | # |
| "DOOLAR" | $ |
| "CARET" | ^ |
| "AMPERSAND" | & |
| "DBLAMPERSAND" | && |
| "ASTERISK" | * |
| "LEFTPAREN" | ( |
| "RIGHTPAREN" | ) |
| "MINUS" | - |
| "UNDERSCORE" | _ |
| "PLUS" | + |
| "EQUALS" | = |
| "LEFTBRACKET" | [ |
| "RIGHTBRACKET" | ] |
| "LEFTBRACE" | { |
| "RIGHTBRACE" | } |
| "COLON" | : |
| "SEMICOLON" | ; |
| "BACKSLASH" | \ |
| "QUOTE" | ' |
| "QUOTEDBL" | " |
| "LESS" | < |
| "GREATER" | > |
| "COMMA" | , |
| "PERIOD" | . |
| "QUESTION" | ? |
| "SLASH" | / |
| "VERTICALBAR" | \| |
| "DBLVERTICALBAR" | \|\| |
| "WWW" | WWW |
| "EMAIL" | Email |

