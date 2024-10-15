# AB_AR_exclude_regular_expressions

**适用于AutoBangumi/ANI-RSS的自用排除正则表达式**

# 说明

**规则都是本人玩了半年autobangumi不断修改，迭代下来的。只放出来自己平时爱订阅的字幕组 ，是个人总结内容，具有时效性。请以个人情况/实际情况为准。(2024.10.15)**

规则如下:

# **桜都字幕组**

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


## **喵萌奶茶屋:**
###### 命名:
- `[繁日双语]:[JPTC].mp4`
- `[间日双语]:[JPSC].mp4`
- `[繁体]:[CHT].mp4`
- `[简体]:[CHS].mp4`

###### 正则表达式:
```text
^(?=.*喵萌奶茶屋)(?=.*(?:繁日双语|繁体))(?!.*LoliHouse).*
```

**`排除说明:[喵萌奶茶屋]+(繁日双语/繁体)+不含LoliHouse`**

{tabs}
{tabs-pane label="例子一"}
 `[喵萌奶茶屋]★07月新番★[从小人物开始的探索英雄谭 / Mob kara Hajimaru Tansaku Eiyuutan][03][1080p][繁日双语][招募翻译]`
{/tabs-pane}
{tabs-pane label="例子二"}
 `[喵萌奶茶屋]★07月新番★[鹿＊子虎视眈眈 / Shikanoko Nokonoko Koshitantan][03][1080p][繁体][招募翻译]`
{/tabs-pane}
{/tabs}


------------


## **北宇治字幕组:**
###### 命名:
- `[繁日内嵌]:[CHT_JP].mp4`
- `[简日内嵌]:[CHS_JP].mp4`
- `[简繁日内封]:[CHS_JP&CHT_JP].mkv`

###### 正则表达式:
```text
^(?=.*\[北宇治字幕组\])(?=.*繁体内嵌).*
```

**`排除说明:[北宇治字幕组]+繁日内嵌`**


{tabs}
{tabs-pane label="例子一"}
 `[北宇治字幕组] 败北女角太多了！ / Make Heroine ga Oosugiru! [01][WebRip][HEVC_AAC][繁日内嵌]`
{/tabs-pane}
{/tabs}



{alert type="info"}
个人说明:由于提供了三语版本，建议直接选择`简繁日内封`，使用`^(?=.*\[北宇治字幕组\])(?=.*内嵌).*`排除内嵌版本
{/alert}


------------


## **MingY:**
###### 命名:
- `[繁日内嵌]:[CHT&JPN].mp4`
- `[简日内嵌]:[CHS&JPN].mp4`
- `[简繁日内封]:[CHS&CHT&JPN].mkv`

###### 正则表达式:
```text
^(?=.*\[MingY\])(?=.*繁体内嵌).*
```

**`排除说明:[MingY]+繁体内嵌`**


{tabs}
{tabs-pane label="例子一"}
 `[MingY] 前辈是伪娘 / Senpai wa Otokonoko [03][1080p][繁日内嵌]`
{/tabs-pane}
{/tabs}


{alert type="info"}
个人说明:由于提供了三语版本，建议直接选择`简繁日内封`，使用`^(?=.*\[MingY\])(?=.*内嵌).*`排除内嵌版本
{/alert}


------------


## **❀拨雪寻春❀:**
###### 命名:
- `[繁日内嵌]:[CHT_JPN].mp4`
- `[简日内嵌]:[CHS_JPN].mp4`
- `[简繁日内封]:[CHI_JPN].mkv`

###### 正则表达式:
```text
^(?=.*\[\❀拨雪寻春\❀\])(?=.*繁日内嵌).*
```

**`排除说明:[❀拨雪寻春❀]+繁日内嵌`**


{tabs}
{tabs-pane label="例子一"}
 `[❀拨雪寻春❀] 义妹生活 / 义妹生活 / Gimai Seikatsu - 02 [WEBRip][AVC-8bit 1080p][繁日内嵌]`
{/tabs-pane}
{/tabs}



{alert type="info"}
个人说明:由于提供了三语版本，建议直接选择`简繁日内封`，使用`^(?=.*\[\❀拨雪寻春\❀\])(?=.*内嵌).*`排除内嵌版本
{/alert}


------------


## **喵萌奶茶屋&LoliHouse:**
###### 命名:
- `[简繁日内封字幕]:[...SC&TC].mkv`

`说明: 发布作品全为双语字幕，无需要排除`



## **沸羊羊字幕组:**
###### 命名:
- `[简繁内封字幕]:[...SC&TC].mkv`

`说明: 发布作品全为双语字幕，无需要排除`


------------


## **爱恋&漫猫字幕组:**
###### 命名:
- `[繁日双语]:[BIG5][MP4].mp4`
- `[简日双语]:[GB][MP4].mp4`

###### 正则表达式:
```text
^(?=.*\[爱恋\&漫猫字幕组\])(?=.*繁日双语).*
```

**`排除说明:[爱恋&漫猫字幕组]+繁日双语`**


{tabs}
{tabs-pane label="例子一"}
 `[爱恋&漫猫字幕组][7月新番][物语系列 番外 怪物季][Monogatari Series Off Monster Season][02][1080p][MP4][繁日双语]`
{/tabs-pane}
{/tabs}



{alert type="info"}
注意: 爱恋&漫猫字幕组发布的作品通常带有`1080p`和`720p`两个版本。不需要`720p`版本可直接添加**`720p`**规则进行排除
{/alert}


------------


## **Kirara Fantasia:**

{alert type="warning"}
不提供简体中文字幕,仅推荐自备字幕尝鲜
{/alert}


###### 命名:
- **(ABEMA 1280x720 AVC AAC MP4):** `ABEMA源,开头有A爹跳脸,720p分辨率,繁体字幕内嵌`
- **(Baha 1920x1080 AVC AAC MP4):** `巴哈源,开头有A爹跳脸,和谐较少,繁体字幕内嵌`
- **(B-Global 3840x2160 HEVC AAC MKV):** `B站东南亚源,4K超高清分辨率码率高,字幕多国语言内封(有时有中文字幕)`
- **(CR 1920x1080 AVC AAC MKV):** `CR源,1080P分辨率,文件体积较大,码率最高,字幕内封`


{alert type="info"}
说明:开头4-5秒的Aniplex，有时会影响自备字幕，导致画面与字幕不同步，个人觉得很影响观感
{/alert}


###### 正则表达式:
```text
^(?=.*\[Up to 21\°C\])(?!.*\b(?:B\-Global)\b).*
```

**`排除说明:[Up to 21°C]+不含B-Global`**


{tabs}
{tabs-pane label="ABEMA源"}
 `[Up to 21°C] 败北女角太多了！ / Make Heroine ga Oosugiru! - 07 (ABEMA 1280x720 AVC AAC MP4)`
{/tabs-pane}
{tabs-pane label="巴哈源"}
 `[Up to 21°C] 败北女角太多了！ / Make Heroine ga Oosugiru! - 07 (Baha 1920x1080 AVC AAC MP4)`
{/tabs-pane}
{tabs-pane label="B站东南亚源"}
 `[Up to 21°C] 败犬女主太多了！ / Make Heroine ga Oosugiru! - 07 (B-Global 3840x2160 HEVC AAC MKV)`
{/tabs-pane}
{tabs-pane label="CR源"}
 `[Up to 21°C] 败北女角太多了！ / Make Heroine ga Oosugiru! - 07 (CR 1920x1080 AVC AAC MKV)`
{/tabs-pane}
{/tabs}


{alert type="info"}
目前就这些,以后还有再补充
{/alert}
