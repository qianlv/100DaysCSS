### 思路

1. 中间3个圈 input radio 单选，这样用 :checked 伪类切换不同得css, 这里结合 :has
来选择父元素，这样就可以用css来控制了
2. 圆球移动:
    - 用一个单独的div来做圆球，通过 position: absolute 定位, transform: translate(-50%, -50%)
      来定位到中心
    - transition: left 1s 移动
    - 用第一步中 :checked 和 has 选择到圆球，修改 left 的值来移动
3. 背景切换:
    - 3 个 div 不同颜色背景，z-index 控制层级, 保证圆球在最上层
    - 背景 position: absolute 定位, 覆盖父元素,
    - transition: right 1s 控制背景定位, 通过修改 right 的值来移动
    - 通过把背景移动到显示区域左边，使下一层背景显示出来，来实现背景切换
    - 类似2中的圆球移动，通过 :checked 和 has 选择到背景，修改 right 的值来移动

### 问题


### 知识

1. [CSS: checked 选择器](https://www.w3schools.com/css/css_selectors.asp)
2. [CSS: pseduo-classes](https://www.w3schools.com/css/css_pseudo_elements.asp)
3. [CSS: position](https://www.w3schools.com/css/css_positioning.asp)
4. [CSS: transition](https://www.w3schools.com/css/css3_transitions.asp)
