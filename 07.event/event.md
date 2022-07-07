## 事件的基本使用:

1.使用 v-on:xxx 或是@xxx 綁定事件，其中 xxx 是事件名。  
2.事件的調用需配置在 methods 對象中，最終會在 vm 上。  
3.methods 中配置的函數，不要用 arrow function，否則 this 就不會指向 vm 了。  
4.methods 中配置的函數，都是被 Vue 所管理的函數，this 的指向是 vm 或組件實例對象。  
5.@click="demo"和@click="demo($event)"效果一致，但後者可以傳參數
