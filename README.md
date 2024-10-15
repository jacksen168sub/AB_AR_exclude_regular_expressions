# AB_AR_exclude_regular_expressions

**适用于AutoBangumi/ANI-RSS的自用排除正则表达式**

<img alt="autobangumi" src="https://raw.githubusercontent.com/jacksen168sub/AB_AR_exclude_regular_expressions/refs/heads/main/images/AB.jpg"/>
<img alt="ANI-RSS" src="https://raw.githubusercontent.com/jacksen168sub/AB_AR_exclude_regular_expressions/refs/heads/main/images/AR.jpg"/>


# 说明

规则都是本人玩了半年autobangumi不断修改，迭代下来的，同样适用于ANI-RSS的排除规则。
种子标题均来自Mikan Project，可能会与其他种子站存在差异。
这里只放出来自己平时订阅的比较多的字幕组，字幕组不分排名先后 。
纯属个人总结内容，具有时效性。请以个人情况/实际情况为准。(2024.10.15)

---
# 目录:


- [桜都字幕组](#桜都字幕组)
- [喵萌奶茶屋](#喵萌奶茶屋)
- [北宇治字幕组](#北宇治字幕组)
- [MingY](#MingY)
- [❀拨雪寻春❀](#%E6%8B%A8%E9%9B%AA%E5%AF%BB%E6%98%A5)
- [LoliHouse](#LoliHouse)
- [沸羊羊字幕组](#沸羊羊字幕组)
- [漫猫字幕组&猫恋汉化组](#%E6%BC%AB%E7%8C%AB%E5%AD%97%E5%B9%95%E7%BB%84%E7%8C%AB%E6%81%8B%E6%B1%89%E5%8C%96%E7%BB%84)
- [Kirara Fantasia](#kirara-fantasia)

---



# 桜都字幕组

## 命名:
- `[简繁内封]: [CHS&CHT].mkv`
- `[简体内嵌]: [CHS].mp4`
- `[简日内嵌]: [CHS&JPN].mp4`

## 正则表达式:
### [01]正则表达式:

```text
^(?=.*\[桜都字幕组\])(?=.*(?:繁体内嵌|繁日内嵌)).*
```

### 排除说明: `[桜都字幕组]+繁体内嵌/繁日内嵌`

### 例子:

- `[桜都字幕组] 迷宫饭 / Dungeon Meshi [24][1080p][繁体内嵌]`


### [02]正则表达式:

```text
^(?=.*\[桜都字幕组\])(?=.*(?:简体内嵌|简日内嵌))(?!.*1080p@60FPS).*
```

### 排除说明: `[桜都字幕组]+简体内嵌/简日内嵌+非1080p@60fps`

- `[桜都字幕组] 无职转生～到了异世界就拿出真本事～ S2 / Mushoku Tensei S2  [24][1080p][繁体内嵌]`


------------


# 喵萌奶茶屋:

## 命名:
- `[繁日双语]:[JPTC].mp4`
- `[间日双语]:[JPSC].mp4`
- `[繁体]:[CHT].mp4`
- `[简体]:[CHS].mp4`

### 正则表达式:
```text
^(?=.*喵萌奶茶屋)(?=.*(?:繁日双语|繁体))(?!.*LoliHouse).*
```

### 排除说明:`[喵萌奶茶屋]+(繁日双语/繁体)+不含LoliHouse`

### 例子:
 - `[喵萌奶茶屋]★07月新番★[从小人物开始的探索英雄谭 / Mob kara Hajimaru Tansaku Eiyuutan][03][1080p][繁日双语][招募翻译]`
 - `[喵萌奶茶屋]★07月新番★[鹿＊子虎视眈眈 / Shikanoko Nokonoko Koshitantan][03][1080p][繁体][招募翻译]`

------------


# 北宇治字幕组:
## 命名:
- `[繁日内嵌]:[CHT_JP].mp4`
- `[简日内嵌]:[CHS_JP].mp4`
- `[简繁日内封]:[CHS_JP&CHT_JP].mkv`

## 正则表达式:
```text
^(?=.*\[北宇治字幕组\])(?=.*繁体内嵌).*
```

### 排除说明:`[北宇治字幕组]+繁日内嵌`


### 例子:
 - `[北宇治字幕组] 败北女角太多了！ / Make Heroine ga Oosugiru! [01][WebRip][HEVC_AAC][繁日内嵌]`


> 个人说明:由于提供了三语版本，建议直接选择`简繁日内封`，使用`^(?=.*\[北宇治字幕组\])(?=.*内嵌).*`排除内嵌版本


------------


# MingY:
## 命名:
- `[繁日内嵌]:[CHT&JPN].mp4`
- `[简日内嵌]:[CHS&JPN].mp4`
- `[简繁日内封]:[CHS&CHT&JPN].mkv`

## 正则表达式:
```text
^(?=.*\[MingY\])(?=.*繁体内嵌).*
```

### 排除说明:`[MingY]+繁体内嵌`


### 例子:
 - `[MingY] 前辈是伪娘 / Senpai wa Otokonoko [03][1080p][繁日内嵌]`


> 个人说明:由于提供了三语版本，建议直接选择`简繁日内封`，使用`^(?=.*\[MingY\])(?=.*内嵌).*`排除内嵌版本


------------


# ❀拨雪寻春❀:
## 命名:
- `[繁日内嵌]:[CHT_JPN].mp4`
- `[简日内嵌]:[CHS_JPN].mp4`
- `[简繁日内封]:[CHI_JPN].mkv`

## 正则表达式:
```text
^(?=.*\[\❀拨雪寻春\❀\])(?=.*繁日内嵌).*
```

### 排除说明:`[❀拨雪寻春❀]+繁日内嵌`


### 例子:
 - `[❀拨雪寻春❀] 义妹生活 / 义妹生活 / Gimai Seikatsu - 02 [WEBRip][AVC-8bit 1080p][繁日内嵌]`



> 个人说明:由于提供了三语版本，建议直接选择`简繁日内封`，使用`^(?=.*\[\❀拨雪寻春\❀\])(?=.*内嵌).*`排除内嵌版本


------------


# LoliHouse:

## 种子标题常用名称:
- LoliHouse
- 喵萌奶茶屋&LoliHouse

## 命名:
- `[简繁日内封字幕]:[...SC&TC].mkv`

### 说明: 发布作品均为双语字幕，无需要排除



# 沸羊羊字幕组:
## 命名:
- `[简繁内封字幕]:[...SC&TC].mkv`

### 说明: 发布作品均为双语字幕，无需要排除


------------


# 漫猫字幕组&猫恋汉化组:

## 种子标题常用名称:
- 爱恋&漫猫字幕组
- 漫猫字幕社&猫恋汉化组

## 命名:
- `[繁日双语]:[BIG5][MP4].mp4`
- `[简日双语]:[GB][MP4].mp4`

### 正则表达式:
```text
^(?=.*(?:\[爱恋\&漫猫字幕组\]|\[漫猫字幕社\&猫恋汉化组\]))(?=.*繁日双语).*
```

### 排除说明:`[爱恋&漫猫字幕组]/[漫猫字幕社&猫恋汉化组]+繁日双语`


### 例子:
 - `[爱恋&漫猫字幕组][7月新番][物语系列 番外 怪物季][Monogatari Series Off Monster Season][02][1080p][MP4][繁日双语]`
 - `[漫猫字幕社&猫恋汉化组][7月新番][物语系列 番外 怪物季][Monogatari Series Off Monster Season][03][720p][MP4][繁日双语]`



> 注意: 爱恋&漫猫字幕组发布的作品通常带有`1080p`和`720p`两个版本。不需要`720p`版本可直接添加`720p`规则进行排除


------------


## Kirara Fantasia:

搬运组: 基本上不提供简体中文字幕,仅推荐自备字幕进行尝鲜使用


###### 命名:
- **(ABEMA 1280x720 AVC AAC MP4):** `ABEMA源,开头有A爹跳脸,720p分辨率,繁体字幕内嵌`
- **(Baha 1920x1080 AVC AAC MP4):** `巴哈源,开头有A爹跳脸,和谐较少,繁体字幕内嵌`
- **(B-Global 3840x2160 HEVC AAC MKV):** `B站东南亚源,多为1080P偶尔有4K分辨率,字幕多国语言内封(有时有中文字幕)`
- **(CR 1920x1080 AVC AAC MKV):** `CR源,1080P分辨率,文件体积较大,码率最高,字幕内封`


> 说明:开头4-5秒的Aniplex，有时会影响自备字幕，导致画面与字幕不同步，个人觉得很影响观感


###### 正则表达式:
```text
^(?=.*\[Up to 21\°C\])(?!.*\b(?:B\-Global)\b).*
```

### 排除说明:`[Up to 21°C]+不含B-Global`


 - ABEMA源: `[Up to 21°C] 败北女角太多了！ / Make Heroine ga Oosugiru! - 07 (ABEMA 1280x720 AVC AAC MP4)`
 - Baha源: `[Up to 21°C] 败北女角太多了！ / Make Heroine ga Oosugiru! - 07 (Baha 1920x1080 AVC AAC MP4)`
 - B站东南亚源: `[Up to 21°C] 败犬女主太多了！ / Make Heroine ga Oosugiru! - 07 (B-Global 3840x2160 HEVC AAC MKV)`
 - CR源: `[Up to 21°C] 败北女角太多了！ / Make Heroine ga Oosugiru! - 07 (CR 1920x1080 AVC AAC MKV)`


> 目前就这些,以后还有再补充
