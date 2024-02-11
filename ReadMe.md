## Package for create styling dropdown with selector

1. Add following code:
   ``` 
   <div class="ts-dropdown">
     <input name="" type="text" class="ts-dropdown__hidden"value="">
     <div class="ts-dropdown__input-block">
       <input type="text" class="ts-dropdown__input"
        placeholder="Search..">
       <i class="fa fa-solid fa-angle-down"></i>
     </div>
   <ul class="ts-dropdown__content">
     <li value="1">first record</li>
     <li value="2">second record</li>
     <li value="3">third record</li>
   </ul>
    </div>
   ```
2. Edit following styles and connect them

    *Note: you should no change the class names & not edit class '.visible'* 
```
.ts-dropdown {
  position: relative;
  height: 40px;
}
.ts-dropdown__content {
  width: 100%;
  list-style: none;
  overflow: auto;
  border: 1px solid #293D32;
  border-radius: 10px;
  position: absolute;
  background-color: #EFE7DC;
  display: none;
  z-index: 7;
}
.ts-dropdown__content li {
  padding: 6px 10px;
  border: 1px solid transparent;
  border-radius: 10px;
}
.ts-dropdown__content li:hover {
  color: #EFE7DC;
  background-color: #293D32;
}
.ts-dropdown__input {
  padding: 7px 10px;
  background-color: transparent;
  width: 100%;
  font-size: 16px;
  border: 1px solid transparent;
}
.ts-dropdown__input:focus {
  outline: none;
  font-weight: 600;
}
.ts-dropdown__input-block {
  padding-right: 6px;
  display: flex;
  align-items: center;
  border: 1px solid #293D32;
  border-radius: 10px;
  background-color: #EFE7DC;
}
.ts-dropdown__input-block_start {
  margin-top: 20px;
}
.ts-dropdown__hidden {
  display: none;
}

.visible {
  display: block;
}
```   
3. Add fontawesome to header
4. Add script
```
<script src="tsDropdown.bundle.js" type="module" defer></script>
```
5. Enjoy