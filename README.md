# 电脑问题解决库 
主要是搜集使用windows时不太常见或在网上难以搜到答案的问题，如果您要补充，请[提交 issue](https://github.com/ruanyf/weekly/issues)
# Windows

### 🔴WIN11右键菜单“正在加载中” <sup>24H2 26100.3915</sup>
打开[Ccleaner](https://www.ccleaner.com/)，点击左边列表中的“工具”，就会出现已安装程序的列表，删除列表中只有"程序名称"没有"其他信息"的程序
>如果你右键点击菜单会闪烁、跳动，大概率也是这个问题

### 🔴文件无法通过拖至任务栏并由任务栏程序打开 <sup>24H2 26100.3915</sup>
打开注册表“计算机\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System”，右击EnableLUA-修改-将数值数据改为1
>Win11下关闭UAC，造成桌面图标和explorer权限不一致，导致无法使用拖拽打开、拖拽快捷方式到任务栏

### 🔴Windows Hello、指纹、人脸等生物识别功能不支持、不可用 <sup>24H2 26100.3915</sup>
更换权限账户
>使用Administrator账户会导致不支持 Windows Hello、指纹、人脸等生物识别功能
