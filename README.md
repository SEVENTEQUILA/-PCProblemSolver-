# PCProblemSolver 
本项目主要用于搜集和解决使用windows时不太常见或不易解决的问题，如果您要补充或提问，请[提交issue](https://github.com/SEVENTEQUILA/PCProblemSolver/issues/new)。解决方案仅供参考，不具有唯一性和通用性。

<br>
<br>

# Windows

### 🔴WIN11右键菜单“正在加载中” <sub>WIN11 24H2 26100.3915</sub>
打开[Ccleaner](https://www.ccleaner.com/)，点击左边列表中的“工具”，就会出现已安装程序的列表，删除列表中只有"程序名称"没有"其他信息"的程序。
>如果你右键点击菜单会闪烁、跳动，大概率也是这个问题。

<br>

### 🔴文件无法通过拖至任务栏并由任务栏程序打开 <sub>WIN11 24H2 26100.3915</sub>
打开注册表“计算机\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System”，右击EnableLUA-修改-将数值数据改为1。
>Win11下关闭UAC，造成桌面图标和explorer权限不一致，导致无法使用拖拽打开、拖拽快捷方式到任务栏。<sup>[[1]](https://bbs.pcbeta.com/viewthread-2025970-1-1.html)</sup>

<br>

### 🔴Windows Hello、指纹、人脸等生物识别功能不支持、不可用 <sub>WIN11 24H2 26100.3915</sub>
更换权限账户。
>使用Administrator账户会导致不支持 Windows Hello、指纹、人脸等生物识别功能。<sup>[[1]](https://bbs.pcbeta.com/viewthread-2025970-1-1.html)</sup>

<br>

### 🔴使用MPV（包括其延申的MPV_lazy、mpv.net等其他版本播放器）、mpc-be等播放器播放视频时出现黑屏/黑屏闪烁现象 <sub>WIN11 24H2 26100.3915 NVIDIA 4060TI 576.02</sub>
首选方案是直接转到Nvidia 控制面板>管理 3D 设置>程序设置>将媒体播放器的垂直同步设置为开启。<br>其他选项：<br>1.在madVR控制面板中将提前呈现的帧数设置为1（设置为3对某些人也有效）<br>2.或者您也可以尝试在nvidiacp中将低延迟模式设置为开启。<br>3.或者将windows电源选项设置
设置为省电模式
>这个问题早在rtx2000系显卡上就出现过，以前主要问题为播放卡顿，黑屏状况较少。<sup>[[1]](https://forum.doom9.org/)</sup>
