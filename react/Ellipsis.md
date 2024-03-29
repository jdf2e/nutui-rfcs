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


Ellipsis:

| 属性 | 描述 | 类型 | 默认值 | 改动点 |
| --- | --- | --- | --- | --- |
| content | 文本内容 | string | - |  |
| direction | 省略位置 | 'start' | 'end' | 'middle' | end |  |
| rows | 展示几行 | number | 1 |  |
| expandText | 展开操作的文案 | string | - |  |
| collapseText | 收起操作的文案 | string | - |  |
| symbol | 省略的符号 | string | ... |  |
| lineHeight | 容器的行高 | string | number | 20 |  |
| onClick | 文本点击是触发 | -- |  | 阻止冒泡事件，已完成；其他组件需关注。 |
| onChange | 点击展开收起时触发 | -- |  |  |


# 缺点

Props 的改动属于破坏性更新，升级成本比较高

# 备择方案


# 采用策略


# 未解决的问题

