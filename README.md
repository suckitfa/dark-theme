原理：
> color，background作为字体色和背景色可以继承
> 直接对body(最高可视区元素)下手定义一个css类
```css
body.dark-model {
    background:black;
    color:white;
}
```
> js的控制
> 使用classList.toggle('dark-model’)
>  来控制黑白模式的切换
> toggle这玩意就是：'有的变没，没的变有'  => 核心就是遍历classList
```js
    document.querySelector('body').classList('dark-toggle');
```