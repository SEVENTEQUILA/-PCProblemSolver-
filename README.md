# 电脑问题解决库 
主要是搜集使用windows时不太常见或在网上难以搜到答案的问题，如果您要补充，请[提交 issue](https://github.com/ruanyf/weekly/issues)
# Windows  
<table>
  <thead>
    <tr>
      <th style="text-align: center">问题</th>
      <th style="text-align: center">解决方案</th>
      <th style="text-align: center">备注</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: left">win11右键菜单“正在加载中”</td>
      <td style="text-align: left">打开<a href="https://www.ccleaner.com/">Ccleaner</a>，点击左边列表中的“工具”，就会出现已安装程序的列表，删除列表中只有"程序名称"没有"其他信息"的程序</td>
      <td style="text-align: left"></td>
    </tr>
    <tr>
      <td style="text-align: left">文件无法通过拖至任务栏并由任务栏程序打开</td>
      <td style="text-align: left">打开注册表，搜索路径“计算机\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System”，右击EnableLUA-修改-将数值数据改为1</td>
      <td style="text-align: left">Win11下关闭UAC，造成桌面图标和explorer权限不一致，导致无法使用拖拽打开、拖拽快捷方式到任务栏</td>
    </tr>
    <tr>
      <td style="text-align: left">Windows Hello、指纹、人脸等生物识别功能不支持、不可用</td>
      <td style="text-align: left">更换权限账户</td>
      <td style="text-align: left">使用Administrator账户会导致不支持 Windows Hello、指纹、人脸等生物识别功能</td>
    </tr>
  </tbody>
</table>
