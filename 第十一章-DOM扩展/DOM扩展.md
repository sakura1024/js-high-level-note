###Welcome to use MarkDown

### selectAPI选择符    

> 下面两个参数：css选择符       
 
- [x]   操作的对象是document元素对象     
 
document.querySelector('.fl')-- 返回找到的第一个元素---一个对象          
document.querySelectorAll('#top')--返回匹配的所有元素---一个伪数组  
        
- [x]   操作的对象是Element元素对象      
  
var aLIs=oul.querySelectorAll('li').length;   

####   验证操作对象oul是否符合后面参数中给定的选择符，符合返回true，反之返回false          

>  需要注意的是：该方法有浏览器兼容性问题--修改前缀      

console.log(oul.webkitMatchesSelector('ul'));   //true                   