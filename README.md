# BertVisualizationTool
## 110學年度NTNU_CSIE專題研究
主題:自然語言模型(BERT)視覺化<br>
指導教授：王科植 KCWang 教授<br>
時間：2021/07 ~ 2022/06<br>

透過將BERT中各屬性資料視覺化，希望能幫助資料科學家更好的理解、修改BERT的框架，加速其他fine-tune模型的訓練
目前進度：
1.可以繪製[CLS]token中每一 dimension 的值，觀察整體走向來判別此句文本是正向情緒或是負面情感
2.可以比對在不同model下，每一層對於同一文本之attention處理是否相似
    方法：計算兩個model中不同層layer，對於attention權重之歐式距離，假設距離越短者代表兩者所做的處理越相關
    
未來期望：
1.分析768個dimension(bert-base-uncased)中，哪幾層對於"情緒"可能比較相關，當然不排除對於其他屬性做研究
2.提供不同算法計算不同層layer的歐式距離，讓使用者能自行選擇
3.提供其他不同屬性的資料，例如hidden layer中每一層內[CLS]token之變化，並試圖繪製出趨勢
及其他未列出但對於分析BERT有用之資料比對
