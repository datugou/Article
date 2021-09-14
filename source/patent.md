
## 专利原文检索
### WIPO 世界知识产权组织检索平台  
<https://patentscope2.wipo.int/search/zh/search.jsf>  
基本包含全球专利，从申请开始到审查完成的**所有公开文件及信息**。  
  - [X] 可爬，同一 IP 多次访问会触发图像识别验证码（需要回答问题，可以尝试建个库），[验证码破解代码]()。  
  
### EPO 欧洲欧洲专利局检索平台  
<https://worldwide.espacenet.com/patent/>  
基本包含全球专利，从申请开始到审查完成的**所有公开文件及信息**。包含更加详细的**专利家族信息**。  
 
### Google Patents  
<https://patents.google.com/>（要翻墙）  
<https://patents.glgoo.top/>（国内镜像）  
基本包含全球专利，包含**常规专利信息及原文**。

### SIPO 国家知识产权局专利公布与布告平台（中国）  
<http://epub.cnipa.gov.cn/>  
可检索并下载 **CN 专利原文**。  
垃圾。访问速度慢；假设一栋办公楼使用同一个公共网络，办公楼太多人访问，会把办公楼整个 ip 认为是机器人，拒绝所有人访问。
  - [ ] 瑞数加密，可用浏览器模拟爬虫（如 selenium 等），同一 IP 多次访问会将该 IP 封一段时间，贼慢，我一般爬 CN 专利用下面的 RainPat。  

### SIPO 国家知识产权局中国及多国专利审查信息查询  
<http://cpquery.cnipa.gov.cn/>  
可查询专利**审查详细**，如法律状态和于专利局的交互文件等。  
垃圾；访问速度慢；许多按道理需要公开的信息没有公开。
  - [ ] 需要登陆，在图像上点击汉字验证码，访问频率太快会被暂时封 ip？账号？ 

### SIPO 专利检索及分析
<http://pss-system.cnipa.gov.cn/>  
垃圾中的垃圾。  
Chromium 内核浏览器经常会卡死。

### FPO freepatentsonline  
<https://www.freepatentsonline.com/>  
可检索并下载 **US、EP、WO 专利原文**  
  - [X] 随便爬，[代码]()。  
  
### RainPat 润桐专利检索  
<https://www.rainpat.com/>  
没什么特色，主要是爬取信息方便。  
可检索并下载 **CN 专利原文**，CN00000000C 这种 C 版本的专利检索时有问题。  
  - [X] 可爬，需要登陆，每天只能爬取有限数量的专利，累计签到可增加数量限制，[爬虫代码]()，[签到代码]()。  

## 生物序列
已知专利，获取专利中的序列表。  
不是通过序列检索到专利（部分付费数据库有该功能）。

### LENS.ORG
<https://www.lens.org/>  
可获取 WO、US、EP、JP 专利中的序列，fasta 格式。

### WIPO 世界知识产权组织检索平台  
<https://patentscope2.wipo.int/search/zh/search.jsf>  
WO 专利，可在'文件'栏找到序列表 txt 版本；  
US、JP 专利，可在'文件'栏中'已公布申请'列中下载 ZIP 包，解压后可以找到序列表，US 一般是以 S00001.XML 为结尾的文件，记事本打开即可。  
KR 专利，可在'文件'栏中'已公布申请'列中点击 XML，搜索 “SequenceListDocument” 直接复制出来。  
CN 专利，可在'说明书'中最下面找一下，如果是文本可以直接复制出来，有的是图片没法复制。  

- 2010 年之后公布的专利 99% 可以获取文本格式的序列表。  
- 如果专利不能按此方法获取，可以尝试在专利的详情页首页看看同家族的其他专利能否获取，同族专利序列表 90% 是一样的。
  - [X] txt or XML 序列表转 fasta 格式[脚本代码]。
  
