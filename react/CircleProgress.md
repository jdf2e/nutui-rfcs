- 开始日期：2023-05-24
- 目标主要版本：NutUI-React 2.0 / NutUI-React-Taro 2.0
- 参考问题Issues：

# 概括

制定统一的规范，提高组件的使用体验，优化或扩展组件的功能。


# 基本示例

代码示例基本和 NutUI-React 网站给出的一致。


# 动机

- 组件 Props 的指向性不强，从直接感受上不能很好的理解其用途。
- 存在一些冗余的 Props，多个 Props 实现类似的功能。
- 组件之间的 Props 名称不统一，组件 Props 记忆成本高，使用体验不流畅。
- 组件并未清晰划分受控和非受控。
- 样式文件存在冗余内容。


# 详细设计


CircleProgress:

| 属性 | 描述 | 类型 | 默认值 | 改动点 |
| --- | --- | --- | --- | --- |
| progress | 百分比 | number | string | 必传项，无默认值 | 改为 percent，另不建议直接作为children展示。默认展示内容为空。 |
| strokeWidth | 圆弧的宽度 | number | string | 5 |  |
| radius | 半径 | number | string | 50 | 改为 size |
| circleColor | 圆环进度条颜色 | number | string | #fa2c19 | 改为 color |
| pathColor | 圆环轨道颜色 | string | #d9d9d9 | 改为 background |
| strokeLinecap | 圆环进度条端点形状可选值为 square butt | string | round | 可废弃，作为变量加入  不能用css变量，因为是path标签的属性 |
| clockwise | 是否顺时针展示 | boolean | true |  |


# 缺点

Props 的改动属于破坏性更新，升级成本比较高

# 备择方案


# 采用策略


# 未解决的问题

