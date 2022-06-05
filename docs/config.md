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
level:
  def0:
    min: 1
    max: 100
    experience: |
      if check &level <= 15 then {
        math &level * 2 + 7
      } else if check &level <= 30 then {
        math &level * 5 - 38
      } else {
        math &level * 9 - 158
      }
```