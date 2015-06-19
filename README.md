# canvas-info
basic info for canvas


## getImageData

```
var imgData=context.getImageData(x,y,width,height);
```

## putImageData

返回 ImageData 对象，该对象拷贝了画布指定矩形的像素数据

* R - 红色 (0-255)
* G - 绿色 (0-255)
* B - 蓝色 (0-255)
* A - alpha 通道 (0-255; 0 是透明的，255 是完全可见的)

```
var c=document.getElementById("myCanvas");
var ctx=c.getContext("2d");
var imgData=ctx.getImageData(10,10,50,50);
ctx.putImageData(imgData,10,70);
```
