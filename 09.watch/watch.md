## 監視屬性 watch

1.當被監視的屬性變化時，回調函數自動調用，進行相關操作  
2.監視的屬性必須存在，才能進行監視!  
3.監視的兩種寫法  
(1)new Vue 時傳入 watch 配置  
(2)通過 vm.$watch 監視

---

## 深度監視

1.Vue 中的 watch 默認不監測對象內部值的改變(一層)  
2.配置 deep:true 可以監測對象內部值的改變(多層)  
備註:  
(1)Vue 自身可以監測對象內部值的改變，但 Vue 提供的 watch 默認不可以  
(2)使用 watch 時根據數據的具體結構，決定是否採用深度監視。

---

## computed 與 watch 之間的區別

1.computed 能完成的任務，watch 都可以完成  
2.watch 能完成的任務，computed 不一定能完成，例如:watch 可以異步操作

兩個重要的小原則  
1.被 Vue 管理的函數，最好寫成普通函數，這樣 this 的指向才是 vm 或 Vue  
2.所有不被 Vue 所管理的函數(定時器 setTimeOut、ajax 的回調函數)，最好寫成 arrow function，這樣 this 的指向才是 vm 或 Vue。
