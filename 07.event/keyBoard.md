## Vue 常用的鍵盤別名

1.enter  
2.delete (包括 delete backspace)  
3.esc  
4.space  
5.tab(特殊 必須配合 keydown 使用)  
6.up  
7.down  
8.left  
9.right

---

Vue 未提供別名的按鍵，可以使用鍵盤原始的 key 去綁定，但要注意轉為 kebab-case(短橫線命名)

---

系統修飾鍵(用法特殊):ctrl、alt、shift、meta(windows 鍵)  
1.配合 ketup 使用:按下修飾鍵的同時，在按其他鍵，隨後釋放其他鍵，事件才觸發  
2.配合 keydown 使用:正常觸發事件

---

也可以使用 keyCode 去指定具體的按鍵(不建議)

---

Vue.config.keyCodes.自定義鍵名=鍵碼
