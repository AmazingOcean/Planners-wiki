```yaml
database:
  use: SQL
  sql:
    host: 127.0.0.1
    port: 3306
    user: root
    password: 123456
    database: planners

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