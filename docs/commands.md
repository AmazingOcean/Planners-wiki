# 指令概览

> **/planners**指令均可缩写为 **/pl**  
> `<>`内的参数为必填参数, `()`内的参数为可选填参数

|命令                                          |说明                                           |
|:---                                          |:---                                           |
|**基础指令**                                  |                                               |
|/planners                                     |获取插件帮助                                   |
|/planners reload                              |重载插件                                       |
|**职业控制相关**                              |                                               |
|/pl job select `(player)`                     |打开职业选择ui, **必须键入玩家名**             |
|/pl job set `<player>` `<job>`                |为**player**设定为指定职业                     |
|/pl job clear `<player>`                      |将**player**的职业状态清除                     |
|**职业等级相关**                              |                                               |
|/pl level give `<player>` `<value>`           |为**player**给予**value**级                    |
|/pl level take `<player>` `<value>`           |从**player**减少**value**级                    |
|/pl experience(exp) give `<player>` `<value>` |为**player**给予**value**点经验                |
|/pl experience(exp) take `<player>` `<value>` |从**player**减少**value**点经验                |
|**职业技能相关**                              |                                               |
|/pl job skill `<player>`                      |打开技能学习/加点GUI                           |
|/pl job cast `(player)` `<skill>`             |使**player**释放**skill**                      |
|/pl job call `<player>` `<key slot>`          |为**萌芽/龙核**设计, 将技能映射到对应**key slot**上, 此处填**key.yml**中的**快捷键ID**|
|/pl point give `<player>` `<value>`           |为**player**给予**value**技能点                |
|/pl point tale `<player>` `<value>`           |从**player**减少**value**技能点                |
|/pl point set `<player>` `<value>`            |将**player**的技能点设置为**value**            |
|/pl point clear `<player>`                    |将**player**的技能点设置为**0**                |