# OpenMsys2Here

1. `win+R` 输入 `regedit` 打开注册表管理器, 在 `HKEY_CLASSES_ROOT\Directory\Background\shell` 下新建一个项, 命名为msys2, 值的内容是 `Open msys2 here`
2. 在 `HKEY_CLASSES_ROOT\Directory\Background\shell\msys2` 下新建一个项, 命名为 `command `, 值的内容是 `c:\msys64\msys2_shell.bat -where "%V"`

>如果希望和 `Open command window here` 一样 `按住shift+右键` 打开, 为msys2添加两个 `String Value` :
>1. `Extended`
>2. `NoWorkingDirectory`
