## 复数的问题
* ` getElementsByClassName getElementsByClassName()`其中的element必须带"s"
* `var para=document.createElement("p");   
var node=document.createTextNode("This is new.");    
para.appendChild(node);`必须加文本节点，最后添加文本节点。
*对象无法比较

## const定义变量的例外
```javascript
// 您可以创建常量数组：
const cars = ["Audi", "BMW", "porsche"];

// 您可以更改元素：
cars[0] = "Honda";

// 您可以添加元素：
cars.push("Volvo"); 
```
## 正则表达式

* /()/<i:执行对大小写不敏感的匹配><g:执行全局匹配（查找所有匹配而非在找到第一个匹配后停止）><m:执行多行匹配> 
* /[abc],[0-9],[x|y]/i,g,m 
* / \d查找数字,\s查找空白字符,\uxxxx查找以十六进制数 xxxx 规定的 Unicode 字符 /i,g,m

> return 建议不要和后面接的代码换行，会被当成空返回   

以下保留词已被从 ECMAScript 5/6 标准中删除：

1|2|3|4
 |:-: | :-: | :-: | :-:| 
 abstract |	boolean |	byte |	char 
 double |	final |	float |	goto 
 int |	long |	native |	short 
 synchronized |	throws |	transient |	volatile 

## 函数：参数默认
如果调用参数时省略了参数（少于被声明的数量），则丢失的值被设置为：undefined。
有时这是可以接受的，但是有时最好给参数指定默认值
```javascript
function myFunction(x, y) {
    if (y === undefined) {
          y = 0;
          return 0;
    } 
    rentrn x*y;
}
myFunction(5);//没传y进去，所以y=undefined;
```
**不通过** 关键词 **var** 创建的变量总是全局的，即使它们在函数中创建。
