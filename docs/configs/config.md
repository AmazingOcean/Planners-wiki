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
  # 经验组名, 可以添加多个经验组
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