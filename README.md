# RingQ

### 背景：

后渗透场景，杀毒软件落地秒了我的大保健 fscan mimikatz ...  这还让我怎么内网渗透啊？





### 目的：

不用关心怎么实现免杀，也不用浪费时间和精力去对某一款工具进行专项修改达成免杀效果

助力每一位像我这样的脚本小子快速实现免杀，hvv尽快打穿点目标内网

支持bypass 360 火绒 Windows Defender，一键免杀上线CS、fscan、mimikatz ...




### 使用方法：

1. 你的任意exe工具，放在与Create.exe 同文件夹下运行即可，会生成一个混淆的main.txt文件。
   
   <u>*Create.exe 此程序仅用于生成main.txt文件，可能存在报毒(c++你懂的) 添加白名单or虚拟机断网使用都可以。*</u>

   ```
   Create.exe mimikatz.exe
   ```


2. 将main.txt和RingQ.exe上传到目标机器，执行 RingQ.exe ~

   内置反沙箱等等等机制 执行后有些许延迟 耐心一会儿~

   ```
   RingQ.exe
   ```
   ![](https://github.com/T4y1oR/RingQ/blob/main/images/help.gif)

   ![](https://github.com/T4y1oR/RingQ/blob/main/images/image-20240511172315793.png)
   ![](https://github.com/T4y1oR/RingQ/blob/main/images/image-20240511172315791.png)

### **微步**（2024.05.22更新）
![](https://github.com/T4y1oR/RingQ/blob/main/images/image-20240511162750465.png)
### **360**（2024.05.22更新）
![](https://github.com/T4y1oR/RingQ/blob/main/images/360.png)
![](https://github.com/T4y1oR/RingQ/blob/main/images/image-20240511165253870.png)

### **Windows Defender**（2024.05.22更新）
![](https://github.com/T4y1oR/RingQ/blob/main/images/DF.png)

### **卡巴斯基**（2024.05.22更新）
![](https://github.com/T4y1oR/RingQ/blob/main/images/kb.png)

### **火绒6.0**（2024.05.22更新）
![](https://github.com/T4y1oR/RingQ/blob/main/images/huorong.png)



### QVM202 报毒是启发式静态扫描，修改文件资源伪造成正常文件一样即可绕过。

### 添加签名、文件名、图标、属性信息、资源...

![](https://github.com/T4y1oR/RingQ/blob/main/images/Snipaste_2024-05-19_18-15-10.png)

<u>*该报毒不是主程序源码被360干掉，此程序我在2024.01月份就一直在实战中使用。*</u>

![](https://github.com/T4y1oR/RingQ/blob/main/images/Snipaste_2024-05-19_18-54-11.png)

### QVM250（bypass 360 QVM202）

[](https://github.com/T4y1oR/RingQ/QVM250)
![](https://github.com/T4y1oR/RingQ/blob/main/images/QVM250.gif)


<u>*图标支持自定义，存放在QVM250/main文件夹内即可。*</u>






## 承诺无任何后门，放心食用。后续如报毒属于正正正正正常现象，提issues（报毒截图and时间环境信息）耐心等待更新即可。tips:  Star后更新更快！

## 项目仅供进行学习研究，切勿用于任何非法未授权的活动，如个人使用违反安全相关法律，后果与本人无关。



### 更新日志
2024.05.22  QVM250发布，bypass 360QVM202

2024.05.14-21 360QVM202报毒 已更新，这个报毒自行更换图标，添加签名...  ~~如果持续出现这个问题，多点star出个专项bypass QVM202脚本~~ 
           Releases新增RingQ.exe原编译出的main.exe文件，方便大家自定义修改降熵

2024.05.11 项目发布，微步纯绿 企业360云沙箱 火绒   ~~没传VT是为了能大家能用久点，大家随意~~



### TODO

- [ ] 不让我传fscan 直接干掉AV？
- [ ] unhook
- [ ] 远程加载
- [x] bypass QVM202
- [ ] ...

