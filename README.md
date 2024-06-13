**LOLAutomationTools** 是一款 **英雄联盟** 的功能扩展工具；用于帮助玩家在部分因无法腾出双手或需要暂离的场景时进行一些简单的客户端操作以节省少量时间；软件不会过多干预玩家对游戏方面的理解和玩法，所以部分功能仍需要先手动配置（如英雄符文配置），过多的拘束会让人麻木，并失去游戏本身的乐趣；积极快乐游戏，共建和谐环境。

# 功能
- 选用英雄
  - 预选英雄
- 禁用英雄
  - 忽略队选
  - 联组禁用模式
- 随机英雄
- 禁选英雄防退
- 接受对局
  - 延迟接受对局
- 创建对局
- 寻找对局
- 交换功能
  - 随机模式交换英雄
    - 或仅被动接受其他玩家交换英雄
  - 征召模式交换选位
    - 或仅被动接受其他玩家交换选位
  - 交换选位的其他项设置
  - 拒绝非选用英雄交换
  - 拒绝非选位顺序交换
- 跳过称赞页面
- 跳过解锁页面
- 匹配超时检测
- 掷空所有骰子
- 聊天回复控制
  - 离开时回复好友消息
  - 离开时回复对局邀请
    - 离开时拒绝对局邀请
- 英雄选用配置
  - 英雄平衡BUFF
  - 自动应用符文
  - 平衡BUFF发送
  - 符文纠错
  - 锁定英雄(随机模式)
- 自动关闭对局
- 自动重连对局
- 自动领取通行证奖励
- 好友请求处理
  - 批量删除好友
- 生涯背景设置
- 更改召唤师头像
- 更改客户端状态
- 更改状态签名
- 名片段位修改
- 英雄成就点数修改
- 清空佩戴勋章
- 功能键屏蔽
- 战绩查询
  - 战绩发送
  - 对局内开黑检测
  - 玩家对局观战
  - 赛后玩家举报
- 局内喊话
- 黑名单
- 游戏设置同步
- 快捷键设置
- 主题设置
  - 深/浅色主题
  - 自适应主题
  - 自定义主题
  - 背景图片设置
  - 字体自定义

# 功能详情
在查看功能详情之前务必明晰各个页面的名称以及其中包含的功能，并留意每项功能标注的**注意项**，这会使你更容易了解每项功能在做什么或能做什么。

![1](https://github.com/SnxiaLianXin/LOLAutomationTools/assets/36157488/ee34aaca-5178-4d0a-bfe8-8081b8c6ce4e)
![2](https://github.com/SnxiaLianXin/LOLAutomationTools/assets/36157488/2d34690f-f3ee-4ce7-ac26-67844e9cd18d)
![3](https://github.com/SnxiaLianXin/LOLAutomationTools/assets/36157488/15356b49-5014-43fa-8343-9b70dd5f336c)
![4](https://github.com/SnxiaLianXin/LOLAutomationTools/assets/36157488/00a43086-853f-4d72-b3ef-fecb6f889f37)
![5](https://github.com/SnxiaLianXin/LOLAutomationTools/assets/36157488/fd18ff3b-bb05-4e1f-86b7-9e7a8fd5699a)

## 选用英雄
在使用**选用英雄**和**禁用英雄**前，都需要在配置页面进行编辑操作（开关项后面的齿轮按钮）。

分路设置仅在部分有区分选位的对局模式中生效（如 *排位赛* 和 *极限闪击* ），随机仅在 *随机英雄* 模式中生效（如 *极地大乱斗*、*无限乱斗*，禁用英雄配置中不包含随机选项），通用则是其他所有模式中生效（不包含之前列举的模式，这是为了使用规范），在执行自动选用英雄时，将按照**选用英雄**的配置项来进行选用。

![image](https://github.com/SnxiaLianXin/LOLAutomationTools/assets/36157488/25e5bbd7-3365-4c00-bee4-713592b10775)

## 预选英雄
此功能的执行逻辑与**选用英雄**基本一致，区别在于**预选英雄**只会在具有禁用阶段的模式中生效，如 *排位赛* 和部分需要禁用英雄的娱乐模式。

## 禁用英雄
**禁用英雄**配置页面除了正常配置模式外，会有一个**联组模式**，点击右上角切换模式按钮切换禁用模式。

*正常禁用模式*：此模式操作逻辑与**选用英雄**的配置页面一致，在执行自动禁用英雄时，如果没有配置禁用的英雄，将在Ban阶段剩余时间少于10秒时空Ban。

![image](https://github.com/SnxiaLianXin/LOLAutomationTools/assets/36157488/4da594b4-7dee-478a-aacd-bd3f046c84b2)

*联组禁用模式*：配置列表中的项将替换为**选用英雄**配置中的项，在选中一个项时，双击左侧的英雄项来将其添加至英雄的**组**中，在执行自动禁用英雄时，将按照**选用英雄**的配置项顺序来进行禁用，如果所有**选用英雄**的配置项**组**中都没有配置要禁用的英雄，则会按正常禁用模式的逻辑来禁用。

![image](https://github.com/SnxiaLianXin/LOLAutomationTools/assets/36157488/f467a1f3-14f9-42ad-858c-1ae93420c57f)

## 忽略队选
执行自动禁用英雄时跳过队伍预选检测。比如将要禁用**疾风剑豪 亚索**时，队伍中已有队友预选了**疾风剑豪 亚索**，通常情况下会跳过禁用该英雄转而禁用下一项，但如果启用了**忽略队选**选项，将会直接禁用该英雄，不建议启用该项。

> ### 注意项：
> **选用英雄**和**禁用英雄**的配置项中的 *随机* 为特殊项，在左侧选择列表的查找英雄输入框内输入 *随机* 才会显示。在已选英雄列表中，右键项以移除或更改其是否保存至配置中，当项被设置为 *临时的* 将不会保存至配置中，下次启动工具时不会加载该项。

## 接受对局
在匹配到对局后自动接受对局。

## 创建对局
你可以通过**创建对局**按钮来手动创建对局或打开此开关项来自动创建对局。
> ### 注意项：
> *自动创建对局* 需要在功能设置页面选择要创建的对局模式。*手动创建对局* 如果未选择要创建的对局模式，将会创建5V5训练营模式。

## 寻找对局
自动寻找对局，此项仅在对局模式房间中且自身为小队拥有者（房主）时生效。

## 跳过称赞
跳过对局结束时队友的称赞页面。
> ### 注意项：
> 此项会在对局结束后自动称赞自己。觉得自己打得不错？给自己点个赞！

## 跳过结算
跳过对局结束时的等待结算（黑屏转圈加载）或赛后结算页面，并回到对局模式房间中。

## 交换功能
此项开关项为主开关，你还需作其他设置。在**交换功能**配置页面中，设置是否在随机英雄模式中与队友交换英雄或是在征召模式中与队友交换选位（选择英雄的顺序）。

![image](https://github.com/SnxiaLianXin/LOLAutomationTools/assets/36157488/74f5564d-646f-4b3c-967e-cb7d1b65602b)

在**交换功能**的**其他设置**中，你可以设置交换的顺序和兼容模式。

![image](https://github.com/SnxiaLianXin/LOLAutomationTools/assets/36157488/63dd8e00-fa5b-4bef-81c3-774e075a7530)

*交换兼容*：
- 无操作：接受与指定 *顺序* 一致的队友的请求。
- 向下接受：接受 ≤ 指定 *顺序* 的队友的请求。
- 向上接受：接受 ≥ 指定 *顺序* 的队友的请求。
- 范围接受：接受 *顺序* ≤（*指定顺序* - *范围*）和 *顺序* ≥（*指定顺序* + *范围*）的队友的请求。

此外，在**其他设置**中还有两个拒绝交换选项，这两项在**启用时**如果队友请求与你交换英雄或选位时不在判定的条件内将会自动拒绝此次交换请求，**否则**不作任何操作，你可以自行决定是否接受交换。

## 延迟接受对局
在启用**接受对局**选项后，该选项生效。启用此项后，**接受对局**仅会在接受倒计时剩余最后一秒时自动接受对局（受功能执行间隔影响）。

## 禁选英雄防退
启用此项后，会在BP阶段的最后一秒执行**选用英雄**或**禁用英雄**。

*常规模式* 下会执行以下操作：
- Ban：自动禁用 **禁用英雄配置** 列表中的英雄，如果没有，则空Ban。
- Pick：自动选用 **选用英雄配置** 列表中的英雄，如果没有，在部分模式中则会导致退出BP并受到匹配惩罚。

*强制模式* 下除了执行与 *常规模式* 相似的操作之外，会额外执行：
- Pick：如果 **选用英雄配置** 列表中没有英雄，会以以下顺序进行尝试：
1. 从近期20场与当前模式相同的历史对局中（如果有的话）选择第一个近期对局中的英雄
2. 从近期20场历史对局中（如果有的话）选择第一个近期对局中的英雄
3. 从最高的五个成就英雄中（如果有的话）选取一个可用的英雄
4. 如果当前已选择了一个英雄但未锁定，工具会自动锁定该英雄
5. 工具会从可用的英雄中随机选择一个英雄

> ### 注意项：
> 你可以在 *功能设置页面* 来更改**禁选英雄防退**功能的模式设置。

## 匹配超时检测
在匹配队列中超过估计时间指定的值时，自动重新寻找对局。

> ### 注意项：
> 你可以在 *功能设置页面* 来更改**匹配超时检测**功能的超时间隔。

## 掷空所有骰子
此项仅在**随机英雄模式**中生效，如果你还有剩余骰子数，将会自动掷空剩余的骰子。
> 偷偷藏着可不好，对吧？

## 聊天回复控制
此项开关项为主开关，你还需作其他设置。在**聊天回复控制**配置页面中，设置是否在离开时自动回复好友消息或对局邀请（各项默认为启用状态），并设置回复的文本内容。

![image](https://github.com/SnxiaLianXin/LOLAutomationTools/assets/36157488/f80d67a5-772f-4b94-9d1d-fef08a59cb25)

## 英雄选用配置
启用此项后，会在BP阶段显示**英雄选用配置窗口**，用于查看当前选择英雄的**基础属性**、**平衡属性**或调整**符文配置**。此外，你可以在此开关项的后方齿轮按钮进入**英雄选用配置**的**符文配置页面**，在此处也可以查看英雄的**基础属性**和在当前可用娱乐模式中的**平衡属性**（如果有的话），并为其配置在各个模式中可用的符文配置。

**英雄选用配置 - 符文配置**页面</br>
![image](https://github.com/SnxiaLianXin/LOLAutomationTools/assets/36157488/e3291f55-13f8-4ad9-9f76-bded8070c072)

> ### 注意项：
> 如果你要在**符文配置页面**添加或更新英雄的符文配置，需要在游戏客户端的 **藏品 - 符文** 中选择一项符文页编辑并保存后，从右上角更改召唤师技能并按下**添加配置**按钮或是要更新的**符文配置项**中的 *将当前游戏配置更新至此配置* 按钮来添加或更新符文配置。

**英雄选用配置**窗口</br>
![image](https://github.com/SnxiaLianXin/LOLAutomationTools/assets/36157488/02a01cc5-1b52-4aa2-b8e6-18da7219f9d5)

> ### 注意项：
> 在 *随机英雄* 模式中，你可以在**英雄选用配置窗口**的右侧看到锁头形状的开关按钮。启用时，将锁定该英雄，当你执行其他操作（选用英雄池里的英雄、投掷骰子）时将会自动切换回该英雄。此外，你可以从**英雄选用配置窗口**的英雄列表页面查看当前英雄池/队伍中的英雄平衡属性，在 *随机英雄* 模式中，你可以按下鼠标左键来选用这些英雄，按下右键来发送这些英雄的平衡属性；在其他 *娱乐模式* 中仅能使用右键发送平衡属性。

## 自动关闭对局
简单直白，在游戏对局结束播放水晶终结动画时自动关闭游戏进程。

## 自动重连对局
在游戏需要重新连接时尝试进行重新连接。
> ### 注意项：
> 每场对局只会自动执行一次重新连接。

