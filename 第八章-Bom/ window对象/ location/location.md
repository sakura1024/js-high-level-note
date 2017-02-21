###Welcome to use MarkDown
- [x] 改变浏览器位置（下面三行代码作用一样） 

  
window.location.assign('https://www.baidu.com/');            
window.location="https://www.baidu.com “               
location.href="https://www.baidu.com/"                                             
          
- [x] 加载新页面，但是没有回退按钮             

location.replace("https://www.taobao.com/");       

- [x] 重新加载当前页面 

location.reload();    //重新加载当前页面，如果页面自上次请求后，没有改变过，则从缓存中重新加载
location.reload(true);  //强制从服务器重新加载页面          
