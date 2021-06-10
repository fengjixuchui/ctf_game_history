## WTF

这是一个的**CTF历史比赛题目信息**的仓库。

主要是中国国内的知名CTF公开赛，一般不包含校内赛、省内赛、内部赛等比赛信息。

包含比赛信息、题目描述信息、部分比赛题目最终分值等信息。

分享师傅们的writeup链接和一些官方、非官方的writeup文档。

支持题目附件和部分题目源码下载，进行题目复现。只用于学习交流，请勿用作它途。如有侵权，请联系删除。

<br/>

### 更新频率

题目信息及附件会在**比赛结束后**尽快更新（我也不想电脑里总存着一堆附件）

如果比赛需要提交wp，一般是**wp提交时间截止后**。

如果发现网盘链接失效可以联系我补发。

<br/>

## 附件下载

每场比赛附件的网盘链接，在对应赛题信息的顶部“附件链接”中。

同时支持百度网盘、腾讯微云、蓝奏云，下载方式请根据个人条件自行选择。

<!-- 每个比赛单独分享链接而不是所有附件一个链接的原因：-->
<!-- 1. 由于放在单个文件夹，偶尔由于不明原因某个附件被ban导致整个分享链接失效-->
<!-- 2. 蓝奏云分享不能套文件夹，分享的文件夹里的文件夹会不显示-->
<!-- 3. 方便下载，快速定位题目附件-->

### writeup

比赛信息中包含部分wp相关网络连接。

writeup文档文件网盘链接如下（内容相同，任选其一）：

> 链接：https://pan.baidu.com/s/1GxQ7t7FoufCMzyhfV726Aw 提取码：hdxw
> 
> 链接：https://share.weiyun.com/LuJAO0cZ 密码：blyfoa
> 
> 链接：https://t1m.lanzous.com/b0af582sj 密码:hdxw

<br/>

## 网盘说明

目前以下所有网盘的上传账号都没有开通会员，配置均为普通用户级别，受限较大

### 百度网盘（非会员下载限速，单文件限制小于4G）

开通了百度网盘会员的用户，建议优先使用百度网盘下载

**文件名敏感词**：yrs（如easyRSA.zip、babyRSA.zip）

文件名包含敏感词会导致分享链接失效

<br/>

### ~~腾讯微云（非会员上传限速，总容量较小）~~

**由于容量较小，从2021年3月22日开始改用阿里云盘替代**

<br/>

由于未开会员，容量只有10G，所以**大于100M的附件一般不会保存到微云**。

分享文件**UNCTF/1910245db14014309ed.zip**显示违规，申诉失败，这个文件微云没存

<br/>

### 阿里云盘

2021年3月22日后的附件会上传到阿里云盘，以前的的附件不再补传。

目前阿里云盘不支持分享功能，描述暂略。

<br/>

### 蓝奏云（限制文件类型和单文件大小）

**2021年06月起单文件超过100M的附件不再上传蓝奏云。**

~~由于蓝奏云限制单个文件最大为100M，经过测试连续上传大于50M单文件会有20%的文件上传失败，所以**对于蓝奏网盘大于100M的附件进行了切割，切分成48M的单个文件（<font color="red">下载时不要下一部分啊喂</font>）**。~~

~~切分方式是直接截取连续的字节，切分和拼接工具在filesplit.py（python3环境），或可或自行按照编号顺序将文件的字节直接拼接。切分后的文件命名方式为`origin_name_[1-n].zip`。~~

例如：

```bash
# 原文件 = file.7z = 276M

python3 filesplit.py -s /mnt/file.7z

# 经过切分后得到
file_1.7z = 48M
file_2.7z = 48M
file_3.7z = 48M
file_4.7z = 48M
file_5.7z = 48M
file_6.7z = 36.7M

# 还原文件
python3 filesplit.py -c /mnt/file.7z

# 会自动按顺序搜寻/mnt/路径下file_[1-n].7z命名方式的文件，，并自动拼接成file.7z保存到/mnt/路径下
```

~~为了防止切分成过多子文件，**大于400M的附件一般不会存到蓝奏云**。~~

<br/>


## 其他

如有疑问或提供相关资源请联系QQ909712710（备注来源：github-ctf_game_history）或QQ群658858223

~~如果本仓库对您有帮助或者您愿意支持本仓库的更新，欢迎扫码捐助（算了，反正也没人扫）~~

### 相关链接

| 链接                                                        | 说明                                                     |
| ----------------------------------------------------------- | -------------------------------------------------------- |
| [web题目复现](https://github.com/docimg/ctf_history_replay) | 使用docker镜像，已有镜像可以直接获取运行，不定期偶尔更新 |
| [CTF在线工具](https://readflag.cn/)                   | 一些CTF相关的信息收集整理                                |

