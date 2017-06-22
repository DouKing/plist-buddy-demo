
#### 添加字段

/usr/libexec/PlistBuddy -c 'ADD :teamID string 12345678' a.plist

/usr/libexec/PlistBuddy -c 'ADD :compileBitcode bool false' a.plist

#### 添加数组

- 添加 key

> /usr/libexec/PlistBuddy -c 'ADD :list array' a.plist

- 添加 value

> /usr/libexec/PlistBuddy -c 'ADD :list: string item1' a.plist

> /usr/libexec/PlistBuddy -c 'ADD :list: bool false' a.plist

#### 添加字典

- 添加 key

> /usr/libexec/PlistBuddy -c 'Add :Person dict' a.plist

- 添加 value

> /usr/libexec/PlistBuddy -c 'Add :Person:Name string a name' a.plist

> /usr/libexec/PlistBuddy -c 'Add :Person:age integer 20' a.plist

> /usr/libexec/PlistBuddy -c 'Add :Person:money real 100.59' a.plist

> /usr/libexec/PlistBuddy -c 'Add :Person:"a new key" string "a new value"' b.plist

#### 打印

- 打印文件

> /usr/libexec/PlistBuddy -c 'print' a.plist

- 打印数组元素

> /usr/libexec/PlistBuddy -c 'Print :list:0' a.plist

#### 删除字段

> /usr/libexec/PlistBuddy -c 'Delete :teamID' a.plist

#### 修改字段

> /usr/libexec/PlistBuddy -c 'Set :list:0 string "this is item1"' a.plist

> /usr/libexec/PlistBuddy -c 'Set :list:1 true' a.plist

#### 合并

> /usr/libexec/PlistBuddy -c 'Merge b.plist' a.plist


