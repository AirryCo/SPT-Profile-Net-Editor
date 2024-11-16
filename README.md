# SPT-Profile-Net-Editor

本软件是一款SPT存档修改器，和`SPT-AKI-Profile-Editor`不同的是，此软件是通过网络与服务器通信达到修改数据的目的，不依赖本地文件，对于客/服分离的玩家比较友好。由于网络数据的关系，此修改器的修改内容并不是很丰富，如果您想体验更丰富的修改项，此修改器并不适合您，请移步至[SPT-AKI-Profile-Editor](https://github.com/SkiTles55/SPT-AKI-Profile-Editor)。

任何涉及存档修改的工具都有破坏存档的风险。您知晓且应当知晓使用本软件会存在导致存档损坏的风险，特别在网络环境不良好的情况下，所以，在使用本软件前，**请备份好您的存档**。

# 功能列表

已支持的修改和画饼

1. 总览

    ✅等级

    🔲昵称

    🔲版本

    🔲阵营

2. 成就

    ✅一键获取

    🔲单个成就的获取和删除

3. 健康

    🔲修改当前值和上限值

4. 技能

    ✅一键满级

    🔲单个技能升降级

    🔲筛选排列

5. 手册

    🔲一键检视

    🔲愿望单物品增删改

6. 仓库

    6.1 物品属性

    ✅堆叠数量

    ✅战局发现

    🔲耐久度

    6.2 存储位置

    🔲仓库
    
    ✅装备

    🔲任务

    🔲藏身处

7. 任务

    ✅一键完成进行中任务（正常领取奖励）

    🔲单个任务的完成、重新开始

8. 商人

    ✅一键满好感度（非等级）

    🔲一键拥有所有服装

9. 藏身处

    🔲一键升级


## 使用说明

### 登入界面

1. 🛜服务器

    SPT服务器IP或者域名，后面是端口号

2. 🌏语言

    工具内的大多数文本均来自服务器的本地化文件，支持的语言和SPT服务器一致。软件界面仅少部分文字需要翻译，支持简体中文和英语。

    - 从服务器获取

        游戏数据默认配置为简体中文（ch）和英语（en），如果您需要更多的语言支持，请单击此按钮。
3. 👦用户名

    顾名思义

4. 🔑密码

    顾名思义

5. 仅加载本地缓存

    需要之前成功获取过用户数据才可以使用。勾选这个模式将不能修改，仅做数据分析。

6. 登入

    顾名思义

### 主界面

1. 支持的模块

    见上面的功能列表。简单来说，目前健康、手册和藏身处数据无法修改，可以修改

    - 人物等级

    - 技能等级

    - 成就获取

    - 装备物品的堆叠数量

    - 任务达成

    - 商人好感度

    点击标签可以切换不同模块，模块内的布局尽量模仿游戏界面。如果在模块内修改了数据，标签页会多出一个`*`。修改完成后，点击`保存`即可把数据发送给服务器，然后**使用`刷新`或`注销`之后重新登入来查看新数据**。

2. 菜单栏

    1. 功能
       - 一键还原(Ctrl+Z)：还原所有模块的修改。
       - 一键保存(Ctrl+S)：保存所有模块的修改。
       - 显示/隐藏所有修改按钮(Ctrl+H)：顾名思义（本地模式会隐藏按钮，不会显示）。
       - 设置模块排列位置：您可以根据自己喜好选择上下左右。
    2. 关于
       - 关于(Alt+A)：相关注意事项。
       - 使用说明(Alt+H)：打开本界面

3. 刷新&注销

    3.1 刷新：从服务器或本地缓存重新读取数据。

    3.2 注销：顾名思义。

4. 图片地址

    优先从本地获取（路径在软件目录的`./files`）。工具里的图片主要分为两个板块：商人头像和任务图片板块、物品图片板块。其中商人头像和任务图片是从游戏服务器获取的，物品图片则需要自行获取资源（目前我把一些图片放在了[GitHub仓库](https://github.com/AirryCo/eft-images)，截止2024.11.16才800多张，远远不够，本人精力有限，希望有能力的小伙伴发起pr一起完善。🌹）

    - GitHub和游戏服务器

        是否下载：✅商人头像、✅任务图片、✅物品图片。物品图片从GitHub下载，商人头像和任务图片将会从游戏服务器下载。

    - 自定义

        用来替代GitHub，是否下载：✅商人头像、✅任务图片、✅物品图片。注意网址的路径，请参照GitHub

    - 仅使用游戏服务器

        是否下载：✅商人头像、✅任务图片、❌物品图片。商人头像和任务图片将会从游戏服务器下载。如果本地不存在物品对应的图片，则用黄金头套替换。

    - 不要下载任何图片

        是否下载：❌商人头像、❌任务图片、❌物品图片。如果本地没有相应资源，则商人头像<img src=':/traders/default_avarar.png'/>替换；物品图片用黄金头套<img src=':/inventory/item_default.png'/>替换；任务图片不显示；。

5. 总览模块

    等级修改：最大80级，修改完后点`保存`。

6. 成就模块

    6.1 一键达成：勾选`全部达成`然后`保存`。

    6.2 取消勾选`尚未达成`可以隐藏未达成的成就。

    6.3 可以按照达成时间/稀有度进行升序/降序排列。

7. 健康模块

    暂不支持修改。和游戏界面一样，不解释了吧。

8. 技能模块

    1. 一键满级：勾选`全部满级`然后`保存`。
    2. 经验值和游戏界面一样，不解释。
    3. 鼠标移到某个技能/专精上面可以查看详细信息。
    4. 点击下一等级数字下面的按钮，可以切换显示方式，和游戏差不多。

9. 手册模块

    每次使用工具的第一次点开可能会有点久，需要耐心等待。

    1. 暂不支持修改。
    2. 可以选择隐藏愿望单或者未检视物品。
    3. 选中物品条目，可以查看图片及描述。图片不存在则使用黄金头套替换。

10. 仓库

    可以查看/修改物品堆叠数量和是否为战局中发现。双击箱子/胸挂等容器可以查看容器内物品。如果出现一个格子同时被两件物品占用的情况，是武器长度的算法问题，不影响游戏内的数据。

    1. 如果您在图片地址选择了`GitHub`或`自定义`，那么第一次打开容器的时候会比较慢，因为软件要在后台下载图片。之后再打开会快很多。
    2. 物品条目为仓库、装备栏、任务物品栏、藏身处物品栏的最外层物品，也就是说，箱子内的物品不会显示
    3. 打开仓库：只读。
    4. 打开装备栏：可以修改物品的堆叠数量和是否为战局中发现。修改后点击`保存`。
    5. 打开任务物品栏：开发中。
    6. 打开藏身处物品栏：开发中。

11. 任务

     第一次点开可能会有点久，需要耐心等待。

     1. 完成全部进行中的任务：`勾选`并`保存`后，会完成**全部**正在进行的任务，奖励进入游戏后可正常领取。
     2. 和游戏一样，可以按照`任务`、`商人`、`类型`、`地点`、`状态`排序（进度排序开发中）

12. 商人

     显示商人的好感度、总花费。

     1. 好感度全满：`勾选`并`保存`，即可将所有商人的好感度升级至6。**注意是好感度，不是等级。**
     2. 点击商人条目可以查看商人介绍。

13. 藏身处

     暂不支持修改。显示区域等级，点击条目可以查看详细描述。

# 写在最后

您的支持是我更新的最大动力。如果您觉得软件还不错，欢迎点个小星星。

作者：

GitHub: https://github.com/AirryCo

塔科夫中文社区：https://sns.oddba.cn/author/190465

教程分享：

[每日自动构建，SPT开发版/每夜版欢迎使用（win+linux）](https://sns.oddba.cn/140144.html)

[[Linux服务端]linux主机/NAS搭建SPT-Server的教程，使用docker和Linux服务管理的方式](https://sns.oddba.cn/137837.html)



文档版本：v0.2.2-beta Commit:605401c