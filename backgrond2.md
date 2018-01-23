# 背景（Background)

<br>

## background

<br>
### 语法

```
background: <bg-color> <bg-image> <bg-position>/<bg-size> <bg-repeat> <bg-origin> <bg-clip> <bg-attachment> |inherit;
```

- &lt;background-color&gt; ：背景颜色，默认值transparent
- &lt;background-image&gt;：背景图像，默认值none。可用url(…)指定图片地址，“相对地址” 或 “绝对地址”。
- &lt;background-repeat&gt;：背景图像的平铺方式
- &lt;background-attachment&gt; ：背景图是否随页面滚动或固定
- &lt;background-position&gt;/&lt;background-size&gt; ：背景图像的位置/背景图像的大小
- &lt;background-origin&gt;：背景图像的原点。
- &lt;background-clip&gt;: 背景剪裁区域。（整个背景）

<br>

### 说明

检索或设置对象的背景。**复合属性。**

- 一个元素可以设置多重背景图，每组属性间使用逗号分隔；

  背景色 [background-color](http://www.css88.com/book/css/properties/background/background-color.htm)> 不能设置多组。

- 如果设置的多重背景图之间存在着交集（即存在着重叠关系），前面的背景图会覆盖在后面的背景图之上

<br>

### 示例

> 假设要在同一个元素上定义3个背景图像

1、缩写方式：
```
background: #aaa
            url(test1.jpg) no-repeat scroll 10px 20px/50px 60px content-box padding-box,
            url(test1.jpg) no-repeat scroll 10px 20px/70px 90px content-box padding-box,
            url(test1.jpg) no-repeat scroll 10px 20px/110px 130px content-box padding-box;
            
```
注意：①<' [background-color](http://www.css88.com/book/css/properties/background/background-color.htm) '> 只能设置一次;
      ②由于写在前面的背景会叠在之后的背景之上，所以建议将背景色定义在最后一组上，避免背景色将图像盖住。

1.1、拆分方式：
```
background-image:url(test1.jpg),url(test2.jpg),url(test3.jpg);
background-repeat:no-repeat,no-repeat,no-repeat;
background-attachment:scroll,scroll,scroll;
background-position:10px 20px,10px 20px,10px 20px;
background-size:50px 60px,70px 90px,110px 130px;
background-origin:content-box,content-box,content-box;
background-clip:padding-box,padding-box,padding-box;
background-color:#aaa;
```

当定义了多个背景图片，而其他属性只有一个参数值，则表明所有背景图片的该属性都应用同一个参数值。
可以对上面的例子进行缩写：

1.2、拆分的缩写：
```
background-image:url(test1.jpg),url(test2.jpg),url(test3.jpg);
background-repeat:no-repeat;
background-attachment:scroll;
background-position:10px 20px;
background-size:50px 60px,70px 90px,110px 130px;
background-origin:content-box;
background-clip:padding-box;
background-color:#aaa;
```

&nbsp;

-------------------
<br>


## background-color

<br>
