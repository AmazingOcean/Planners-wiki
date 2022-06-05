# config.yml

> 插件基础设置

```yaml
database:
  #当前版本还未完成本地存储功能, 仅限使用SQL存储
  use: SQL
  sql:
    host: 127.0.0.1
    port: 3306
    user: root
    password: 123456
    database: bukkit-plugin

options: {}
# by chemdah
#等级自定义公式
level:
  # 经验组名, 可以添加多个经验组, 对应在职业设置的counter键内
  def0:
    # 最低等级
    min: 1
    # 最高等级
    max: 100
    # 经验公式
    experience: |
      if check &level <= 15 then {
        math &level * 2 + 7
      } else if check &level <= 30 then {
        math &level * 5 - 38
      } else {
        math &level * 9 - 158
      }
```

> #### experience经验公式详解  
> if check &level <= 15 即为当等级<=15时对应的经验公式  
> 
> math &level * 2 + 7分解开看:  
> &level * 2 为当前等级*2  
> +7则为在上面的基础上再+7  
> 
> else if为`不满足if条件则...`的意思  
> else 为`不满足if与else if条件则...`的意思  
> 
> 那么整个经验公式则可以理解为:  
> 等级<=15时的经验公式为 **`level *2 +7`**  
> 等级在16-30级范围内时的经验公式为 **`level *5 -38`**  
> 等级>31时的经验公式为 **`level *9 -158`**