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


Card:

| 属性 | 描述 | 类型 | 默认值 | 改动点 |
| --- | --- | --- | --- | --- |
| imgUrl | 左侧图片Url | string | - |  |
| title | 标题 | string | - |  |
| price | 商品价格 | string | - |  |
| vipPrice | 会员价格 | string | - |  |
| shopDesc | 店铺介绍 | string | - |  |
| delivery | 配送方式 | string | - |  |
| shopName | 店铺名称 | string | - |  |
| prolistTpl | 自定义商品介绍 | reactnode | - |  |
| originTpl | 价格后方自定义内容 | reactnode | - |  |
| shopTagTpl | 店铺介绍自定义 | reactnode | - |  |
| footerTpl | 右下角内容自定义 | reactnode | - |  |


# 缺点

Props 的改动属于破坏性更新，升级成本比较高

# 备择方案


# 采用策略


# 未解决的问题

