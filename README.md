# weekly
用于记录

## 8.1
- [How To Learn Stuff Quickly](https://www.joshwcomeau.com/blog/how-to-learn-stuff-quickly/)
  - 看教程的同时，要动手去做，比如学的时候可以在 codesandbox 里写一些代码
  - 学的过程中要学会记录，用文章说一下自己的心得，有点像那个什么学习法一样
  - 任务分配在每天花一点时间去做，任务完成周期延长，但总时不变。个人的感觉是周期的延长可以有更多时间给你思考，有些东西并不是一下就能理解的

## 8.4 
- 浏览器内部会节流我们的dom操作，但是当我们需要读取dom的属性时，浏览器会强制刷新，以确保我们获得的值是最新的
- dom 读写最好分离
```
// bad
div.style.left = div.offsetLeft + 10 + "px";
div.style.top = div.offsetTop + 10 + "px";

// good
var left = div.offsetLeft;
var top  = div.offsetTop;
div.style.left = left + 10 + "px";
div.style.top = top + 10 + "px";
```
