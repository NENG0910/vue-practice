計算屬性 computed:  
1.定義:要用的屬性不存在，要通過已有的屬性計算而來。  
2.原理:底層借助了 Object.defineproperty 方法提供的 getter 和 setter。

3.get 函數什麼時候執行?  
(1)初次讀取的時候會執行一次  
(2)當依賴的數據發生改變時會再一次調用

4.優勢:與 methods 實現相比，內部有緩存機制(複用)，效率更高，調試方便。

5.備註:
(1)計算屬性最終會出現在 vm 上，直接讀取即可。  
(2)如果計算屬性要被修改，那必須寫 set 函數去響應修改，且 set 中要引起計算時依賴的數據發生改變。
