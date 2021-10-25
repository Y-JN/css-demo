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
  /*由于是flex,所以当父元素的区域缩放时,其子项的缩放优先于width/height */
```

****
间距的写法 :
- 使用margin
- 使用padding
- 格式化宽度,设置top/right/bottom/left
- 其他
```css
/* 不仅格式化了div的宽高(让其100%),而且相当于设置了margin:100px */
div{
  position:absolute;
  top: 100px;
  right: 100px;
  bottom: 100px;
  left: 100px;
}
```


****
[输入框效果来源](https://www.bilibili.com/video/BV14D4y1Q74V)
[扭曲的光圈](https://www.bilibili.com/video/BV11L4y1z71E)
> 一个div元素 - 设置具体宽高, 给div元素加上两层光圈:写两个伪类, 加上动画:改变光圈颜色和大小, 再加上一层svg滤镜, 使其光圈扭曲
> 如果想要一个光圈效果:设置box-shadow:0 0 10px 颜色,inset 0 0 10px 颜色;即可
> 如果想要一个动态光圈效果:改变光圈大小(模糊半径)和改变颜色即可