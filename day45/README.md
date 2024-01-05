## 思路

1. 用 svg polyline 画出矩形
2. 一个polyline 做背景, 一个 polyline 做动画
3. 动画 polyline 的 stroke-dasharray 切割2端，一段white部分显示，一段black部分隐藏
4. 用 stroke-dashoffset 控制动画的移动

## 参考

1. [SVG 描边](https://svg-animation-booklet.vercel.app/chapter5.html)
2. [stroke-dasharray 参数](https://medium.com/@waiting7777/%E7%94%A8-svg-stroke-dasharray-%E5%AE%8C%E6%88%90%E5%80%92%E6%95%B8%E8%A8%88%E6%99%82%E5%99%A8-4e76a69e5b87)
