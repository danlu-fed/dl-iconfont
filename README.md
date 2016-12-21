# dl-iconfont

计划规整一套用于丹露网交易平台的图标字体。
暂时还未投入使用。
持续更新，如果你想使用的话请保持关注。

# usege

#### unicode引用

unicode是字体在网页端最原始的应用方式，特点是：

* 兼容性最好，支持ie6+，及所有现代浏览器。
* 支持按字体的方式去动态调整图标大小，颜色等等。
* 但是因为是字体，所以不支持多色。只能使用平台里单色的图标，就算项目里有多色图标也会自动去色。

> 注意：新版iconfont支持多色图标，这些多色图标在unicode模式下将不能使用，如果有需求建议使用symbol的引用方式

unicode使用步骤如下：

> 以下路径为你的字体存放的地址，暂时不提供cdn服务，拷贝font下字体文件使用。

1. 设置font-dace来引入字体

``` css
@font-face {
  font-family: 'dl-icon';
  src: url('iconfont.eot');
  src: url('iconfont.eot?#iefix') format('embedded-opentype'),
  url('iconfont.woff') format('woff'),
  url('iconfont.ttf') format('truetype'),
  url('iconfont.svg#dl-icon') format('svg');
}
```

2. 定义iconfont样式

``` css
.dl-icon{
  font-family:"dl-icon" !important;
  font-size:16px;font-style:normal;
  -webkit-font-smoothing: antialiased;
  -webkit-text-stroke-width: 0.2px;
  -moz-osx-font-smoothing: grayscale;
}
```

3. 应用

``` html
<i class="dl-icon">&#x33;</i>
```

打开[这个](https://danlu-fed.github.io/iconfont/)页面来查看有哪些图标可以使用。