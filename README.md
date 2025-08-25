# 全部收集自tg群组大佬，仅为留着自用。

## 通知-资源入库

```text
{
        'title':'📂 已入库{{ file_count }}个文件\n'
                '{{ title_year }}',
        'text': '{% if season_episode %}\n📺 集数： {{ season_episode }}{% endif %}'
                '{% if category %}\n🎭 类别： {{ category }}{% endif %}'
                '{% if releaseGroup %}\n👥 小组： {{ releaseGroup }}{% endif %}'
                '{% if resource_term %}\n🌟 质量：{{ webSource }}{{ resource_term }}{% endif %}'
                '{% if audioCodec %} {{ audioCodec }}{% endif %}'
                '\n💾 大小： {{ total_size }}'
                '{% if err_msg %}，以下文件处理失败：{{ err_msg }}{% endif %}'
    }
```

## 通知-资源下载

```text
{
    'title': '📥 开始下载\n{{ title_year }}',
    'text': '{% if download_episodes %}\n📦 季集： {{ season_fmt }} {{ download_episodes }}{% else %}\n📦 季集： {{ season_episode }} {% endif %}'
            '{% if pubdate %}\n🕒 时间： {{ pubdate }}{% endif %}'
            '{% if category %}\n🎭 类别： {{ category }}{% endif %}'
            '{% if site_name %}\n🌐 站点： {{ site_name }}{% endif %}'
            '{% if resource_term %}\n🌟 质量：{{ webSource }}{{ resource_term }}{% endif %}'
            '{% if size %}\n💾 大小： {{ size }}{% endif %}'
            '{% if seeders %}\n🌱 做种： {{ seeders }}{% endif %}'
            '{% if labels %}\n️🏷 标签： {{ labels }}{% endif %}'
            '{% if original_name %}\n📛 名称： \n{{ original_name }}{% endif %}'
            '{% if description %}\n\n📝 描述： {{ description }}{% endif %}'
  
}
```

## 通知-添加订阅

```text
{
        'title': '🎞 {{ title_year }} {% if season %}{{season_fmt}}{% endif %} 已添加订阅',
        'text': '{% if vote_average %}✨ 评分：{{ vote_average }}/10{% endif %}'
                '{% if category %}\n📽 类型：{{ category }}{% endif %}'
                '{% if username %}\n👾 用户：{{ username }}{% endif %}'
                '\n🔗 链接：{{ __mediainfo__.detail_link }}'
                '{% if actors %}\n🤵 参演：{{ actors }}{% endif %}'
                '{% if overview %}\n\n🍿 简介：\n{{ overview }}{% endif %}'
    }
```

## 通知-订阅完成

```test
{
        'title': '🎞 {{ title_year }} {% if season %}{{season_fmt}}{% endif %} 已完成订阅',
        'text': '{% if vote_average %}✨ 评分：{{ vote_average }}/10{% endif %}'
                '{% if username %}\n👾 用户：{{ username }}{% endif %}'
                '\n🔗 链接：{{ __mediainfo__.detail_link }}'
                '{% if overview %}\n\n🍿 简介：\n{{ overview }}{% endif %}'   
}
```

## 自定义规则

```text
[{"id":"Complete","name":"完结","include":"(全|共)\\d+(集|期)|完结|合集|Complete","exclude":""},{"id":"filterGlobal","name":"全局过滤","include":"","exclude":"(?i)日语无字|先行|MiniBD|DIY原盘|iPad|UPSCALE|AV1|BDMV|RMVB|CAMRip|DVD|vcd|480p|OPUS"},{"id":"filerGroup","name":"组过滤","include":"","exclude":"(?i)SubsPlease|Up to 21°C|VARYG|TELESYNC|NTb|sGnb|BHYS|HDSWEB|DBD|HDH|COLLECTiVE|SRVFI|YTS.MX|HDSPad"},{"id":"filterMovie","name":"电影体积过滤","include":"","exclude":"","size_range":"0-1000000"},{"id":"filterSeries","name":"剧集体积过滤","include":"","exclude":"","size_range":"0-10240"},{"id":"Crunchyroll","name":"CR源","include":"CR|Crunchyroll","exclude":""},{"id":"Netflix","name":"NF源","include":"Netflix|NF","exclude":""},{"id":"AMZN","name":"AMZN源","include":"AMZN|Amazon","exclude":""},{"id":"HQ","name":"高码","include":"HQ|高码|EDR","exclude":""},{"id":"DVP8","name":"杜比P8","exclude":"^(?!.*HDR).*(DV|dovi|DoVi)"},{"id":"DDP","name":"杜比音轨","include":"DDP|DD+","exclude":""},{"id":"WhiteList","name":"白名单","include":"\\b(Oldboys|GTR|RO|Telesto|CatEDU|PbK|Rainbaby|Ao|BMDru|c0kE|cfandora|jsum|RNML|FraMeSToR|ADE|CHD|CMCT|Sunny|WiKi|PTer|MTeam|FRDS|UBits|FROGE|beAst|Dream|BeiTai|RLeaves|R²|PTH|HDChina|LHD|ZONE|btshd|ADWeb|HHWEB|CHDWEB|CMCTV|TJUPT|OurTV|PTerWEB|MWeb|UBWEB|FROGWeb|QHstudIo|DBTV|RLWeb|LeagueWEB|HDCTV|ZWEX|ZmWeb|Kitsune|NTb|playWEB|BYNDR|FLUX|ETHEL|EDITH|VARYG|HONE|YingWEB|OPS|AilMWeb|ARiC|喵萌奶茶屋|豌豆字幕组|爱恋字幕社|漫猫字幕社|北宇治字幕组|云光字幕组|织梦字幕组|千夏字幕组|极影字幕社|风之圣殿字幕组|风车字幕组|银色子弹字幕组|熔岩动画|MingYSub|枫叶字幕组|诸神字幕组|AKito|秋人|霜庭云花Sub|轻之国度字幕组|星空字幕组|离谱Sub|雪飘工作室|拨雪寻春|新Sub|MCE汉化组|極彩字幕组|氢气烤肉架|悠哈璃羽字幕社|桜都字幕组|SweetSub|LoliHouse|&VCB-Studio|VCB-Studio&|7³ACG|幻之字幕组|魔穗字幕组|澄空学园|LittleBakas!|白恋字幕组|动漫国字幕组|FSD字幕组|FSD粉羽社|一只出格君|猫恋汉化组|OPFans枫雪动漫|GM-Team|康复重症监护室字幕组|SilverBullet|APTX4869|幻樱字幕组|永恒译制|咪梦字幕组|NEO·QSW)\\b"},{"id":"PreferenceGroup","name":"优先组","include":"ADWeb|HHWEb|FROGWeb|ADE|FROGE"}]
```

## 优先级规则组

```text
[{"name":"前置过滤","rule_string":"filterGlobal& !BLU & !3D &WhiteList&DVP8","media_type":"","category":""},{"name":"动画电影","rule_string":" SPECSUB & 4K & BLURAY & H265 &filterMovie> CNSUB & 4K & BLURAY & H265 &filterMovie> CNSUB & 4K & BLURAY &filterMovie> CNSUB & 1080P & BLURAY &filterMovie> CNSUB & 4K &filterMovie> CNSUB & 1080P &filterMovie","media_type":"电影","category":"动画电影"},{"name":"华语电影","rule_string":" 4K & BLURAY & H265 > 1080P & BLURAY > 4K &HQ&DDP> 4K &HQ> 4K > 1080P ","media_type":"电影","category":"华语电影"},{"name":"外语电影","rule_string":" SPECSUB & 4K & UHD & H265 & DOLBY &filterMovie> SPECSUB & 4K & UHD & H265 &filterMovie> SPECSUB & 1080P & BLURAY &filterMovie> CNSUB & 1080P & BLURAY &filterMovie> SPECSUB & 4K & WEBDL & DOLBY &filterMovie> CNSUB & 4K & WEBDL & DOLBY &filterMovie> SPECSUB & 1080P & WEBDL &filterMovie> CNSUB & 1080P & WEBDL &filterMovie> CNSUB &filterMovie","media_type":"电影","category":"外语电影"},{"name":"日番","rule_string":" BLURAY & H265 &PreferenceGroup& 1080P > BLURAY & H265 & CNSUB & 1080P > BLURAY & CNSUB & 1080P > WEBDL &PreferenceGroup& 1080P &Crunchyroll> WEBDL &PreferenceGroup& 1080P &AMZN>PreferenceGroup&Netflix& 1080P & WEBDL > WEBDL &PreferenceGroup& 1080P > 1080P & CNSUB > CNSUB ","media_type":"电视剧","category":"日番"},{"name":"欧美漫","rule_string":" BLURAY & H265 & CNSUB > BLURAY & CNSUB > WEBDL & CNSUB > CNSUB ","media_type":"电视剧","category":"欧美漫"},{"name":"国漫","rule_string":" 4K &PreferenceGroup&DDP> 4K &PreferenceGroup> 1080P &PreferenceGroup> 4K > 1080P > 720P ","media_type":"电视剧","category":"国漫"},{"name":"纪录片","rule_string":" 4K & BLURAY > 1080P & BLURAY > 4K > 1080P ","media_type":"电视剧","category":"纪录片"},{"name":"综艺","rule_string":" 4K &PreferenceGroup&Complete> 4K &PreferenceGroup> 1080P &PreferenceGroup> 1080P ","media_type":"电视剧","category":"综艺"},{"name":"国产剧","rule_string":" 4K & UHD > 1080P & BLURAY > 4K & WEBDL &HQ&PreferenceGroup&filterSeries> 4K & WEBDL & HDR &PreferenceGroup> 4K & WEBDL &PreferenceGroup> 4K & WEBDL > 1080P & WEBDL > 4K > 1080P ","media_type":"电视剧","category":"国产剧"},{"name":"欧美剧","rule_string":" 4K & BLURAY & SPECSUB &filterSeries> 4K & BLURAY & CNSUB &filterSeries> 1080P & BLURAY & SPECSUB &filterSeries> 1080P & BLURAY &filterSeries& CNSUB > 4K & CNSUB &filterSeries> 1080P & CNSUB &filterSeries> CNSUB &filterSeries","media_type":"电视剧","category":"欧美剧"},{"name":"日韩剧","rule_string":" SPECSUB & 1080P & BLURAY &filterSeries> CNSUB & 1080P &filterSeries> 1080P & CNSUB &filterSeries> CNSUB &filterSeries","media_type":"电视剧","category":"日韩剧"},{"name":"现场","rule_string":" CNSUB & 4K > CNSUB & 1080P > 4K > 1080P > !720P ","media_type":"电影","category":"现场"}]
```

## 🎬电影重命名

```text
{{title}}{% if year %}({{year}}){% if tmdbid%} [tmdb={{tmdbid}}]{% endif %} {% endif %}/{{title}}{% if year %}({{year}}){% endif %}{% if part %}-{{part}}{% endif %}{% if videoFormat %} - {{videoFormat}}{% endif %}{{fileExt}}
```

## 📺电视剧重命名

```text
{{title}}{% if year %}({{year}}){% endif %}{% if tmdbid%} [tmdb={{tmdbid}}]{% endif %}/Season {{season}}/{{title}} {% if year %}({{year}}){% endif %} - {{season_episode}}{% if part %}-{{part}}{% endif %}{% if episode %} - 第 {{episode}} 集{% endif %}{{fileExt}}
```

## 自定义共享识别词（复制粘贴➡️插件）

```text
https://raw.githubusercontent.com/Putarku/MoviePilot-Help/main/Words/TV.txt
https://raw.githubusercontent.com/Putarku/MoviePilot-Help/main/Words/anime.txt
https://raw.githubusercontent.com/Putarku/MoviePilot-Help/main/Words/general.txt
https://raw.githubusercontent.com/Putarku/MoviePilot-Help/main/Words/2025.01.txt
https://raw.githubusercontent.com/Putarku/MoviePilot-Help/main/Words/2025.split.txt
https://raw.githubusercontent.com/Putarku/MoviePilot-Help/main/Words/anime.txt
```

## 自定义占用符

```text
\b(简繁内封|简繁日内封|简繁日英内封|简繁官字内封|官简内封|简日双语|简体内封|简体内嵌|繁体内嵌|简英双语|简繁外挂|简体|DoVi|HQ|HDR10|hq|60FPS|d\+fps|d\+FPS)\b
```

## 文件整理屏蔽词

```text
__\w{6}/
\[((TV|BD|\bBlu-ray\b)?\s*CM\s*\d{2,3})\]
\[Teaser.*?\]
\[PV.*?\]
#\[\d{2}.\d\]
\[NC[OPED]+.*?\]
\[S\d+\s+Recap(\s+\d+)?\]
\b(CDs|SPs|Scans|Preview|EXTRA|ScreenShot|Menu|Bonus|映像特典|映像|Special Ending Movie|specials|特典CD|Menu|Logo|Preview|WiKi.sample|UHD.SAMPLE|/mv)\b
\b(NC)?(Disc|片头|OP|OVA|OAD|ED|Advice|Trailer|BDMenu|片尾|PV|CM|Preview|MENU|Info|EDPV|SongSpot|BDSpot)(\d{0,2}|_ALL)\b
名侦探柯南特典合集|名侦探柯南剧场版22周年合集|名侦探柯南真人版|系列合集|特别篇合集|加更
```

## 自定义制作组/字幕组

```text
喵萌奶茶屋
银色子弹字幕组
AI-Raws
SweetSub
LoliHouse
VCB-Studio
7³ACG
Snow-Raws
NTb
FLUX
RLWeb
Breeze@Sunny
Rain@Sunny
RLeaves
Nest
MWeb
UBWEB
FROG
```