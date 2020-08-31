## D3CTF

> https://d3ctf.io/
>
> 比赛时间：11月22日20:00－11月24日20:00
>
> 初赛平台：https://platform.d3ctf.io/#/user/login
>
> 部分题目源码仓库：https://github.com/D-3CTF/D3CTF-2019-Challenges



## Writeup

官方WP已发布：https://www.anquanke.com/post/id/193939

[2019-D3CTF_WP.pdf](../writeup/2019-D3CTF_WP.pdf)



## 附件链接

链接：https://pan.baidu.com/s/19YEQC7OpPSzDrcws1NLkzA 提取码：hdxw

链接：https://share.weiyun.com/FVqjNtlB 密码：uj6rqi

外链:https://t1m.lanzous.com/b0aeszung 密码:hdxw



## WEB
### Showhub(880.7pt,2sloved)
> Showhub is a fashion-focused community built on a self-developed framework.
> [Download this framework here](/d3ctf/www_4beeb1dada.tar.gz)
> Notice:scanner is useless
> Hint1:The password of admin is strong enough, so you can only try to modify it.
> 题目地址 http://004cabd84a.showhub.d3ctf.io



### easyweb(460.16pt,21sloved)
> source code is in [attachments](/d3ctf/www_b4e607f625.zip)
> 题目地址 http://0eec3c4959.easyweb.d3ctf.io



### babyxss(1000pt,0sloved)
> xss? seriously? 
>
> Check out the CSP plz
> admin is using the latest Chrome released.
> You may want to look into chrome://components
> portable sodium chloride
> 题目地址 https://85856f986c.babyxss.d3ctf.io



### d3guestbook(1000pt,0sloved)
>hint:You don't need to fuzz, just audit the front-end code
>题目地址 http://fb4aa0e977.d3guestbook.d3ctf.io



### fake onelinephp(588.74pt,11sloved)
> None.
> 题目地址 http://ce2baa434e.fakeonelinephp.d3ctf.io

题目源码
```
<?php ($_=@$_GET['orange']) && @substr(file($_)[0],0,6) === '@<?php' ? include($_) : highlight_file(__FILE__);
```

服务器路径：C:\Users\w1nd\Desktop\web\nginx-1.17.6\html\index.php



### ezts(965.54pt,1sloved)
> ORM $eq Not SQLi? 
> Note: The challenge will be reset every 60 seconds and the profile data will be reset as well. User will be retained. 
> Hint1: [source code](/d3ctf/src_125387345b.zip)
> Hint2: root privilege can be gained with sudo.
> 题目地址 http://770af96c40.ezts.d3ctf.io



### ezupload(1000pt,0sloved)
> webroot in /var/www/html
> Notice:scanner is useless
> hint1: webroot changes every 10 mins
> hint2: glob
> hint3: https://www.php.net/manual/en/language.oop5.decon.php
> 题目地址 http://9943aafc2c.ezupload.d3ctf.io



## PWN
### lonely_observer(965.54pt,1sloved)
> [https://d3ctf-pwn-1256301804.cos.ap-shanghai.myqcloud.com/lonely_observer.zip](/d3ctf/lonely_observer.zip)
> 题目地址 
> nc 49.235.24.33 11492



### basic_basic_parser(965.54pt,1sloved)
> [https://d3ctf-pwn-1256301804.cos.ap-shanghai.myqcloud.com/basic_basic_parser.zip](/d3ctf/basic_basic_parser.zip)
> 题目地址 
> nc 106.54.67.184 29440



### unprintableV(571.79pt,12sloved)
> [https://d3ctf-pwn-1256301804.cos.ap-shanghai.myqcloud.com/unprintableV.zip](/d3ctf/unprintableV.zip)
> 题目地址 
> nc 212.64.44.87 13568




### new_heap(880.7pt,2sloved)
> (attachments updated at 11/24 01:06) [https://d3ctf-pwn-1256301804.cos.ap-shanghai.myqcloud.com/new_heap-updated.zip](/d3ctf/new_heap-updated.zip)
> 题目地址 
> nc 49.235.24.33 25325



### ezfile(965.54pt,1sloved)
> [https://d3ctf-pwn-1256301804.cos.ap-shanghai.myqcloud.com/ezfile.zip](/d3ctf/ezfile.zip)
> Hint: fileno
> 题目地址 
> nc 212.64.44.87 21220



### babyrop(556.09pt,13sloved)
> [https://d3ctf-pwn-1256301804.cos.ap-shanghai.myqcloud.com/babyrop.zip](/d3ctf/babyrop.zip)
> 题目地址 
> nc 106.54.67.184 13305




### knote(627.3pt,9sloved)
> [https://d3ctf-pwn-1256301804.cos.ap-shanghai.myqcloud.com/0f462a0c93.zip](/d3ctf/0f462a0c93.zip)
> 题目地址 
> nc 49.235.24.33 9999




### knoteV2(820.35pt,3sloved)
> We have found that the challenge knote has an unintended solution, and it's deadly simple ;-(. We fixed it and came up with this knote v2. 
> (Sorry about that, we promise the author will be "punished" badly (๑•̀ω•́๑) ) 
> [https://d3ctf-pwn-1256301804.cos.ap-shanghai.myqcloud.com/knote-v2-d41d8cd98f.zip](/d3ctf/knote-v2-d41d8cd98f.zip)
> 题目地址 
> nc 49.235.24.33 9998




## REV
### Ancient Game V2(702.6pt,6sloved)
> The ancient game strikes back.
> 题目地址 https://d3ctf-rev-1256301804.cos.ap-shanghai.myqcloud.com/dddb4cc54c/chall_46837d2ca1.html



### ch1pfs(965.54pt,1sloved)
> a poor fs with an easy format
> 题目地址 [https://d3ctf-rev-1256301804.cos.ap-shanghai.myqcloud.com/11facab435/14a0193712561fdd62cec1e627469536.zip](/d3ctf/14a0193712561fdd62cec1e627469536.zip)



### easy_dongle(820.35pt,3sloved)
> This is an easy hardware dongle which use UART(USB to TTL serial) to decrypt the encryption executable software. 
> The .zip archive contains two files, "easy_dongle.elf" is a ELF executable file of host computer and "dongle.bin" is the binary file which download to the slave device. 
> Note that slave device is STM32F103C8T6. 
> (Pay attension to memory mapping, instruction set and interrupt vector table of STM32F103)
> 题目地址 [https://d3ctf-rev-1256301804.cos.ap-shanghai.myqcloud.com/5b6e74e278/dc4659c3f1.zip](/d3ctf/dc4659c3f1.zip)



### KeyGenMe(965.54pt,1sloved)
> Hey, this is a license-protected pushBox game. Feel free to play~
> 题目地址 [https://d3ctf-rev-1256301804.cos.ap-shanghai.myqcloud.com/17099a2b51/e043e39470.tar.gz](/d3ctf/e043e39470.tar.gz)



### Machine(965.54pt,1sloved)
> Long time ago, a machine was built for math calculating. Nowadays, it's redesigned to verify the specific flag. However, it works sometimes slowly. Can you help me? Note: This machine only works under Android 4.4 ~ 6. And every time the machine is running, only the first check is working normally.
> 题目地址 [https://d3ctf-rev-1256301804.cos.ap-shanghai.myqcloud.com/901a797b4f524b5570a62afaab0a7a2f.apk](/d3ctf/901a797b4f524b5570a62afaab0a7a2f.apk)



### SIMD(1000pt,0sloved)
> hint1:Please pay attention to vpgatherdd
> hint2:Try to find the round key
> 题目地址 [https://d3ctf-rev-1256301804.cos.ap-shanghai.myqcloud.com/3dc343a5cc1a010d187fe9092f918f98.zip](/d3ctf/3dc343a5cc1a010d187fe9092f918f98.zip)



### disappeared_memory(1000pt,0sloved)
> My name is Jim Shown. Ten years ago, I was a Master of Windows, and now I'm a great great great OZone pentester. Accidentally, I got this dump file in some ways. It's said that this memory dump contains a secret. After analysis, I found a suspicious process, ...but something went wrong. I have never encountered this kind of problem ten years ago, that must be something new of Windows 10 ;( 
>
> P.S. Jim Shown and OZone are just fake names ;) 
> hint1: Find compressed memory!
> 题目地址 [https://d3ctf-rev-1256301804.cos.ap-shanghai.myqcloud.com/lucky_a7cb7f6a1f589bc67ca6f4ac4b67862c.dmp.tar.gz](/d3ctf/lucky_a7cb7f6a1f589bc67ca6f4ac4b67862c.dmp.tar.gz)



## Crypto
### Common(702.6pt,6sloved)
> Are you familiar with Wiener's attack?
> 题目地址 [https://d3ctf-crypto-1256301804.cos.ap-shanghai.myqcloud.com/d13bc5b68b/task_1f8dadca6e.py](/d3ctf/task_1f8dadca6e.py)



### Bivariate(820.35pt,3sloved)
> The Coppersmith method, proposed by Don Coppersmith in the Wild, is a method to find small integer zeroes of univariate or bivariate polynomials modulo a given integer. The method uses the Lenstra–Lenstra–Lovász lattice basis reduction algorithm (LLL) to find a polynomial that has the same zeroes as the target polynomial but smaller coefficients.
> 题目地址 [https://d3ctf-crypto-1256301804.cos.ap-shanghai.myqcloud.com/b078b70185/task_a9372a32cf.py](/d3ctf/task_a9372a32cf.py)



### Noise(702.6pt,6sloved)
> Listen...The secret is...M2@...f*#...z()I!(...3;J...Hello?...really noisy here...God bless you get it... 
> attachment: [noise.py](/d3ctf/noise_6bf8bcee73.py)
> 题目地址 
> nc 129.226.75.200 25780



### sign2win(735.09pt,5sloved)
> Do you want the flag? You can get the server code here [server_56219b1c73.py](/d3ctf/server_56219b1c73.py)
> 题目地址 
> nc 129.226.163.141 12233



### babyecc(607.15pt,10sloved)
> Have you ever studied number theory?
> mid_a is the minimum positive integer that satisfies S(mid_a) = {1}
> 题目地址 [https://d3ctf-crypto-1256301804.cos.ap-shanghai.myqcloud.com/b3b5ff9301/ef1d7befd4.sage](/d3ctf/ef1d7befd4.sage)




## MISC
### c+c(965.54pt,1sloved)
> This is a lite version of a great galgame (a.k.a. Visual Novel) written by Romeo Tanaka. Hope you enjoy it.
> 题目地址 [https://d3ctf-misc-1256301804.cos.ap-shanghai.myqcloud.com/53bb5f6f0c6d562a1ffd01729d69a541.tar.gz](附件太大没上传)



### Find Me?(820.35pt,3sloved)
> Find the password . flag must be d3ctf{.+} .
> 题目地址 [https://d3ctf-misc-1256301804.cos.ap-shanghai.myqcloud.com/2bce3dfe7daf59c33e80d2894f147006.zip](/d3ctf/2bce3dfe7daf59c33e80d2894f147006.zip)



### Vera(880.7pt,2sloved)
> For some reason, big hacker w1nd has been arrested by us. During the search on his computer, we found a strange file that could not be opened. Someone guessed that it had been encrypted, but W1nd refused to provide the password. Near the computer, we also found [a book](https://play.google.com/store/books/details?id=kCTMFpEcIOwC) with a bookmark. Specifically, the bookmark is on page 13 of this book. Maybe this is the length of the password. 
> hint: VeraCrypt ISBN
> 题目地址 [https://d3ctf-misc-1256301804.cos.ap-shanghai.myqcloud.com/774103b49e/800ba1872d.file](/d3ctf/800ba1872d.file)




### Welcome To D^3CTF!(10pt,383sloved)
> IRC, or TG, or QQ, that is the question. 
> Hint: You can find the flag in our group / channel.
> 题目地址 https://platform.d3ctf.io

QQ群(532023069)公告
```
d3ctf{w3ee3eeeeE3e1comE-t0_d3cTF}
```



### bet2loss_v2(773.46pt,4sloved)

> Public and open source projects are free to start, maintain, and contribute to. Thanks @[LoRexxar](https://github.com/LoRexxar/HCTF2018_bet2loss)
> hint:settings.py is the KEY to win, and tells you HOW to get the flag.
> 题目地址 http://416dcac539.bet2lossv2.d3ctf.io



### D^3CTF 2019 Survey(571.79pt,12sloved)
> We are willing to hear from you!
> 题目地址 https://forms.gle/FyHV1SF1NEufk5c89

```
d3ctf{thanks_for_your_response!}
```