css效果

****
css配色网站: 
[Gradihunt](https://gradihunt.com/)
[CoolHue](https://webkul.github.io/coolhue/)
[WebGradients](https://webgradients.com/)
[css Scales](https://bennettfeely.com/scales/)
[uiGradients](https://uigradients.com/#ColorsOfSky)
[Gradient](https://gradient.shapefactory.co/) - 喜欢

****
居中写法:
- 需要确定宽高,给当前盒子写样式
```css
  /* 居中wrapper,但是需要确定宽高 */
  .wrapper{
    width: 300px;
    height: 300px;
    position: absolute; 
    left: 0;
    right: 0;
    bottom: 0;
    top: 0;
    margin: auto;
  }
```
- 不需要确定宽高,给当前盒子的父元素写样式
```css
  /* 居中wrapper,不需要wrapper确定宽高 */
  body{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    .wrapper{...}
  }
```

****
[输入框效果来源](https://www.bilibili.com/video/BV14D4y1Q74V)