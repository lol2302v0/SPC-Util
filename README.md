**This document is written in Chinese. If you don’t know Chinese, please use a translation software to translate me, or open the [English 'ReadMe' Document](./ReadMe_EN.md)**

# SPC-Util

SPC 的 多功能工具。

专业的PvZ数据修改辅助工具。（针对游戏PvZ）

是最优秀的PvZ修改辅助工具，拥有其他工具说拥有、或未拥有的功能，诸如 RTON 编码与解码、加密与解密(当时，这个功能只会在游戏彻底停止运营后才可能公布)、DZ、PAK、RSGP、RSB数据包的解包与打包、PAM与FLASH动画之间的相互转换、等等。

# SPC-Util 与 PvZ-Tool

PvZ-Tool 是本人的首个工具，与SPC-Util一样，他是针对PvZ的数据修改辅助工具，他只提供安卓版本，并且难以使用，甚至我本人如今也不会使用了。

PvZ-Tool 是除了 SPC-Util 与 QuickBMS 之外，市面上唯一能够进行PvZ2数据包打包的工具，且他的打包功能比QuickBMS的回包强大许多，因此，它在国内外的PvZ2数据修改者中具有不小的流传度。

值得一提的是，PvZ-Tool的初始公开版本并不含有数据包打包的功能，原本这个功能只是我个人是私用品。后来，我将带有限制的程序传给了Justin-Gdnz并告诫他不要流传出去，后来，JustinGdnz发现了这个程序所定限制的漏洞并将之传播开来，数据包的打包不再是“秘密”，这就是最初流传的带有数据包打包功能的 PvZ-Tool，直到2019年底，我将我几年前给予JustinGdnz的工具正式公开在Bilibili网站与百度贴吧。

必须声明的是，我的任何程序（PvZ-Tool、SPC-Util）一直都是、未来也会是免费、公开的，有一些别有用心之人，通过得到免费的PvZ-Tool、修改其程序，篡改作者名字、甚至是篡改打包功能中所定义的“固定内容”(包含了作者我的名字)（这些很容易修改，因为这个程序没有经过任何处理、加固），将至卖出高价出售（据我所知，有些人通过25$美元购买了这个免费工具）、赚取经济收益。这令我极为不齿。

SPC-Util 脱胎于 PvZ-Tool。在 PvZ-Tool 完成一段较长的时间后，本人想要为其制作新功能，但由于其执行效率、代码质量过低（PvZ-Tool是作者初学C语言制作的程序），思考之下，我放弃了PvZ-Tool，并使用C++语言重写了PvZ-Tool的大多数功能，将之命名为 SPC-Util。SPC 取自我的网名 SmallPC，Util 意为 Utility，即：多功能工具。

SPC-Util(与PvZ-Tool) 的各个功能，是本人独立研究与原创、或是与他人一同研究、或是通过互联网上查找到的知识，一步步完成的。每行代码都是作者的心血。

# 捐赠

如果你喜欢我的软件，并且有自己可支配的金钱，可以捐赠一定的金钱奖赏，激励我制作愈加完善的SU工具，感谢每位捐赠者。

当然，如果你不进行任何捐赠，你依然可以使用SU正式版的任何功能，我说过：本程序永远是免费、公开的。

捐赠时，请尽量备注你的网名，自1.14.4版本开始，每次发布新版本SU时，我都会将捐赠名单写入SU程序界面上。

## 捐赠渠道

微信(WeChat)：

![Image](./donate/wechat.png)

支付宝(AliPay)：

![Image](./donate/alipay.jpg)

QQ钱包(QQ)：

![Image](./donate/qq.png)

# 名 人 名 言（确信）（开玩笑

> MF (PvZ2-IZM系列作者之一) 说：“不知道SPCUtil的人就相当于没搞过修改（确信）。”、“没su系列的话IZM地图都做不出来，硬改json我不如去死。”  

> CZ (PvZ2-Shuttle系列作者) 说: “SPCUtil是史上最强大最方便的回包工具。”、“su的帮助真的不小，把不可能变为了可能，超赞。”  

# 如何使用？

1. 在 Release 界面下载最新版本的 exe文件 与 environment.zip 环境配置文件。
2. 解压 environment.zip 到文件夹 D:/SPCUtil 中。
3. 移动 exe文件 到文件夹 D:/SPCUtil 中.
4. 拖拽待处理的文件到SU的exe文件图标上，例如 rton文件、json文件、rsb/obb文件、等。
5. 完成第四步后，SU程序就会启动，弹出可选的处理方法，通过输入数字选择你要使用的功能，在程序运行完毕后，你就能在同一地方看到新生成或处理过的文件。

# SU都能用来做什么？

1. 基础的操作，例如 RTON与JSON 文件的相互转换。
2. 解包与打包“数据包”文件，支持 PAK（一代PC端的数据包） & DZ (一代安卓端曾经使用过的数据包格式), RSGP(二代的数据包子包，有人称其为：pgsr) & RSB(二代数据包，也可用 OBB、RSB.SMF 等文件后缀).
3. 解码、编码PAM文件(二代的专有动画数据文件，类似于一代的 reanim 文件)，可在PAM与FLASH动画文件之间相互转换，也可转换成适用于CSS动画的JSON数据文档、并使用SU拓展工具：SU动画查看器，查看解析出的动画。只有转换成FLASH动画才能够被修改并转换回PAM文件。

4. 其他功能，用户自行探索.
