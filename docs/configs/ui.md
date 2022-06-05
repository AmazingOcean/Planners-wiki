# ui.yml

> 插件GUI配置

```yaml
job:
  title: '请选择职业'
  rows: 1
  job-slots: [ 1,2,3,4,5,6,7 ]
  icon-#:
    slots: [ 0,8 ]
    material: BLACK_STAINED_GLASS_PANE
    name: ''

skill-backpack:
  title: 'Skill | Backpack'
  rows: 4
  skill-slots: [ 10,11,12,13,14,15,16,19,20,21,22,23,24,25 ]
  addon-info:
    - '&a当前绑定快捷键 {{ meta skill shortcut }}'
    - '&a左键打开技能面板'
    - '&a右键切换/设置快捷键'
  icon-#:
    slots: [ 0,1,2,3,4,5,6,7,8,9,17,18,26,27,28,29,30,31,32,33,34,35 ]
    material: BLACK_STAINED_GLASS_PANE
    name: ''

shortcut-selector:
  title: 'Shortcut Selector'
  rows: 3
  key-slots: [ 10,11,12,13,14,15,16 ]
  key-icon:
    name: '{name}'
    material: NAME_TAG
  icon-#:
    slots: [ 0,1,2,3,4,5,6,7,8,9,18,19,20,21,22,23,24,25,26 ]
    material: BLACK_STAINED_GLASS_PANE
    name: ''
faceplate:
  title: '{name} | faceplate'
  rows: 6
  item-slot: 19
  item-slots: [13,14,15,16,22,23,24,25,31,32,33,34]
  next-icon:
    slot: 49
    material: ANVIL
    name: '升级'
    lore:
      - ''
      - '&c升级到下一级所需技能点数 &f{point}'
      - ''
  icon-#:
    slots: [ 0,1,2,3,4,5,6,7,8,9,10,11,12,17,18,20,21,26,27,28,29,30,35,36,37,38,39,40,41,42,43,44,45,46,47,48,50,51,52,53 ]
    material: BLACK_STAINED_GLASS_PANE
    name: ''
```