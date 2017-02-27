###Welcome to use MarkDown

### selectAPI选择符    

> 下面两个参数：css选择符       
 
- [x]   操作的对象是document元素对象     
 
document.querySelector('.fl')-- 返回找到的第一个元素---一个对象          
document.querySelectorAll('#top')--返回匹配的所有元素---一个伪数组  
        
- [x]   操作的对象是Element元素对象      
  
var aLIs=oul.querySelectorAll('li').length;  
  
- [x]   querySelector和querySelectorAll都不是动态查询，文档结构动态改变时，querySelector和querySelectorAll对应的结果不会再次改变；---不会引起性能问题
而getElementById、getElementsByClassName等则是动态查询的，文档改变时，他们对应的值也会改变---会引起性能问题	   
  

####   验证操作对象oul是否符合后面参数中给定的选择符，符合返回true，反之返回false          

>  需要注意的是：该方法有浏览器兼容性问题--修改前缀      

console.log(oul.webkitMatchesSelector('ul'));   //true    


###   element.classList属性

ex:<div class="bd user disabled div containClass removeClass toggle1Class">

- [x]  element.classList的length属性 
	oDiv.classList.length;         

- [x]  add(class1, class2, ...)-----在元素中添加一个或多个类名         
	oDiv.classList.add('addClass');          

- [x] contains(class)----返回布尔值，判断指定的类名是否存在。----true - 元素包已经包含了该类名,false - 元素中不存在该类名         
	var bool=oDiv.classList.contains('containClass');            

- [x] remove(class1, class2, ...)---移除元素中一个或多个类名。         
	oDiv.classList.remove('removeClass');         

- [x] toggle(class, true|false)----	在元素中切换类名。         
	第一个参数为要在元素中移除的类名，并返回 false。          
	如果该类名不存在则会在元素中添加类名，并返回 true。          
	
	第二个是可选参数，是个布尔值用于设置元素是否强制添加或移除类，不管该类名是否存在。例如：         
	移除一个 class: element.classList.toggle("classToRemove", false);          
	添加一个 class: element.classList.toggle("classToAdd", true); 
	
	oDiv.classList.toggle('toggle1Class');
### 焦点管理
- [x] document.activeElement----引用DOM中获得焦点的元素，返回获得焦点的元素
- [x] document.hasFocus()---判断某个元素是否获得焦点，返回true或者false
              