# quant_project

* 選擇權策略(主要為衍金第12章策略)

+ 模式
  + 跑回歸預測價格上漲下跌(幅度)、波動程度(C.I.)
  + 參考回歸預測結果，選擇策略
    + 波動大、預測上漲下跌
      (1) 多頭逆轉組合、空頭轉換組合
      (2) 多頭空頭價差組合
      (3) 買進勒式組合
    + 波動小(進入盤整)、使用選擇權策略(Butterfly, ... etc.)
      (4) 賣出勒式組合
    (波動率：https://wizardforcel.gitbooks.io/python-quant-uqer/content/194.html
     
     GARCH模型：https://zhuanlan.zhihu.com/p/21962996
               https://uqer.datayes.com/v3/community/share/57aac592228e5b9b95a88999)
  
  + 目前使用策略  
      + 第一部分：追多頭、空頭趨勢，使用多頭逆轉組合、空頭轉換組合
      + 第二部分：一樣追趨勢，但改用有限風險的價差組合
      + 第三部分：不追趨勢，使用勒式組合
      + 第四部分：找盤整期，使用勒式組合獲利
      + 第五部分：勒式混和(3+4)
      
      + 補：
        + 追趨勢：波動率大加上 momentum 方向(code: squeeze and momentum)
        + 買進勒式：波動率大
        + 賣出勒式：波動率小
          (關於波動率大小的標準測試後再行決定)
          
    
    最後Performance metrics(如何呈現? e.g. sharpe ratio, and more)
    
+ 分配工作
  + Coding
  + 文檔
  + 策略
  
+ 時間分配
  + 第一周
    + Coding
      拿到Data後，做好架構
    + 文檔
      主要篇幅設計(標題、選擇權策略內容)
    + 策略
      策略選擇(不同情況考慮使用何種策略)
  + 第二周
    (待定
