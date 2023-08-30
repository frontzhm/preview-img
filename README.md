# previewImg

预览和缩放图片，无依赖，纯js，适合任意框架

安装

```shell
npm i preview-img-js
```

使用

```js
import {preivew-img} from 'preview-img';
previewImg('https://blog-huahua.oss-cn-beijing.aliyuncs.com/blog/code/typora-user-images/image-20221016081802807.png')
// previewImg(img元素)
```

效果图：![preview_img](https://blog-huahua.oss-cn-beijing.aliyuncs.com/blog/code/preview_img.png)
![preview_img](https://blog-huahua.oss-cn-beijing.aliyuncs.com/blog/code/preview_img.gif)

## 参数设置

```js
options = {
  isListenWheel: false, // 是否监听滚轮事件,默认不监听
  startZoom: 1, // 缩放比例，默认值为1，表示不缩放
  isClickShadeClose: true, // 是否点击遮罩层关闭,默认为true
  colorMask: 'rgba(0,0,0,.7)', // 遮罩层的颜色,默认为rgba(0,0,0,.7)
  hasCloseBox: true, // 是否有关闭按钮,默认为true
  hasActionBox: true, // 是否有操作按钮,默认为true
  hasAnimateWhenIsImgEl: false, // 当传入值是el是否有动画,默认为false
  afterCloseCallback: null, // 关闭之后的回调
  afterScaleCallback: null, // 改变尺寸之后的回调
}
previewImg(url,options)
```


