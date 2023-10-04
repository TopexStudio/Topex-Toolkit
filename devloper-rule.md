## Topex-Toolkit开发准则

1. 软件UI控件必须使用标尺软件量，由**LAGSNES**负责。

2. 软件的初衷是工具箱，在添加除`Topex Toolkit > Tools`也就是**工具箱功能**以外的Feature，需要开发组成员共同讨论

3. Topex Toolkit的UI层级划分为**主界面 > 主界面子UI > 子程序**。  
   子程序是在主界面以外的非单独功能(例如:桌面管理器、网络管理器)，应当加上`窗口_启动`当做加载界面。层级划分示例如下:

   ```markdown
   Topex Toolkit - 主界面
   	Tools
   ↓		
   桌面管理器、时钟管理器...
   ```

希望各位Topex-Toolkit开发者可以严格遵守该准则