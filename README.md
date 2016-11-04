# jQuery-Tabledit

## 新增的參數
``` 
rowKey 

cxcore_class:'cxcore_class'  
    
cxcore_elseselect:'cxcore_elseselect'

cxcore_elseinput:'cxcore_elseinput'

```

## 新增的函數

```

onEditClick

```

## rowKey and onEditClick 用法
1. 設定 rowKey 將會使 tr 的ID 增加前綴字串


```
$("#table").Tabledit({
                url: 'xxxxxx.xxxxx.xxxx',
                rowKey: 'userID_' ,
                columns: {
                   //......略 
                },
                onEditClick:function(){
                  console.log('onEditClick()');
                  //處理編輯按鈕點擊後的事件
                  
                },
                //......略 
```
## cxcore_class and cx_core_else 用法
1. 新增自定義的 class 如cxcore_class=" xxxxxxx "
2. 新增自定義之自定義元素字串 cx_core_else=' xxxx=xxxx '
3. 而 參數 cxcore_class 和cx_core_else 都是可以自定義的。

```

<td cxcore_elseinput='' cxcore_class="time_picker " cx_core_else='data-plugin="datepicker"' >{{ $VAL['time'] }}</td>

```







## License
1. 修改自 作者：markcell所開發的jQuery-Tabledit https://github.com/markcell/jQuery-Tabledit 
2. Code released under the MIT license.
