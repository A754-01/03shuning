# 苏宁移动端首页（rem 布局）



## 项目类型：静态页面





## 1.技术选型

1.1.方案：rem布局



## 2.搭建相关文件夹结构



# 3.设置样式文件

3.1.设置公共样式文件common.less

```css
// 设置常见的屏幕尺寸 修改里面的html文字大小
// html{font-size: 50px;}这句一定要写到最上面
html {
  font-size: 50px;
}

// 我们此次定义的划分分数为 15 
@num: 15;

// 320
@media screen and (min-width: 320px) {
  html {
    font-size: (320px / @num);
  }
}

// 360
@media screen and (min-width: 360px) {
  html {
    font-size: (360px / @num);
  }
}

// 375
@media screen and (min-width: 375px) {
  html {
    font-size: (375px / @num);
  }
}

// 384
@media screen and (min-width: 384px) {
  html {
    font-size: (384px / @num);
  }
}

// 400
@media screen and (min-width: 400px) {
  html {
    font-size: (400px / @num);
  }
}

// 414
@media screen and (min-width: 414px) {
  html {
    font-size: (414px / @num);
  }
}

// 424
@media screen and (min-width: 424px) {
  html {
    font-size: (424px / @num);
  }
}

// 480
@media screen and (min-width: 480px) {
  html {
    font-size: (480px / @num);
  }
}

// 540
@media screen and (min-width: 540px) {
  html {
    font-size: (540px / @num);
  }
}

// 720
@media screen and (min-width: 720px) {
  html {
    font-size: (720px / @num);
  }
}

// 750
@media screen and (min-width: 750px) {
  html {
    font-size: (750px / @num);
  }
}
```



3.2.把 common.less 导入 index.less

```less
@import "common.less"
```

3.3.设置body样式

```css
body{
  min-width: 320px;
  width: 15rem;
  margin: 0 auto;
  line-height: 1.5;
  font-family: Arial, Helvetica;
  background-color: whitesmoke;
}
```

