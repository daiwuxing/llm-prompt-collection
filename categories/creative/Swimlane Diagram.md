# SVG Swimlane Diagram Generator

## Metadata
- **Created**: 2024-02-26
- **Model**: Claude3.7Sonnet
- **Category**: Creative
- **Tags**: Diagram, SVG, Visualization, Design, Flowchart

## Prompt
```
请创建一个SVG格式的泳道图(Swimlane Diagram)，需要满足以下规范：

1. 基础布局规范：
a) 尺寸设置：
- 根据泳道数量和复杂度确定合适的viewBox尺寸
- 泳道宽度根据内容量动态调整，但保持成比例
- 预留适当的顶部标题区域（建议占总高度的5-10%）
- 确保足够的图形间距和留白
b) 视觉分层：
- 使用渐变或纯色背景区分泳道
- 标题区域使用深色背景突出
- 泳道之间使用明确的分割线(建议0.5-1px)
- 图形元素层级要高于背景
2. 连接点位置规范：
a) 不同形状的标准连接点：
矩形连接点：
- 水平：左右边的中点 (x ± width, y + height/2)
- 垂直：上下边的中点 (x + width/2, y ± height)
圆形连接点：
- 四个主要位置：0°, 90°, 180°, 270°
- 计算公式：
  * 右：(cx + r, cy)
  * 左：(cx - r, cy)
  * 上：(cx, cy - r)
  * 下：(cx, cy + r)
菱形连接点：
- 四个顶点
- 或各边中点
b) 连接点注释格式：
<!-- connection-points
    top: x,y
    right: x,y
    bottom: x,y
    left: x,y
-->
3. 连接线设计规范：
a) 基本原则：
- 优先使用直线连接
- 避免线条交叉
- 保持45°或90°的转角
- 遵循从左到右、从上到下的流向
b) 连接策略：
- 同泳道：优先垂直连接
- 跨泳道：水平或折线连接
- 复杂路径：使用正交连接线
c) 特殊情况处理：
- 不同大小图形：保持中点对齐
- 避让其他元素：使用折线或贝塞尔曲线
- 多条交叉线：调整路径或使用桥接
4. 图形布局规范：
- 保持适当的垂直和水平间距
- 图形大小要协调统一
- 确保视觉平衡和对称
- 预留足够的连接线空间
5. 文字样式规范：
- 图形内文字居中对齐
- 标题文字要醒目
- 字体大小要适中
- 确保良好的可读性
6. 可视化增强：
a) 颜色规范：
- 背景色使用低饱和度色彩
- 重要节点使用高对比度色彩
- 相关元素使用相近色系
- 确保颜色具有足够对比度(建议>4.5:1)
b) 视觉层次：
- 主要流程突出显示
- 次要信息适当弱化
- 使用阴影或高光突出重点
- 区分前景和背景层次
7. 注释和标识：
a) 必要注释：
- 关系类型标注
- 重要节点说明
- 流程方向指示
- 特殊情况说明
b) 图例说明：
- 提供图形类型说明
- 说明线条样式含义
- 标注颜色代表含义
- 补充必要的业务说明
8. 最佳实践：
a) 代码组织：
- SVG元素合理排序
- 使用注释标识各部分
- 保持代码整洁有序
- 图形ID命名规范
b) 交互考虑：
- 预留悬浮效果空间
- 为可能的动画留出余地
- 考虑响应式适配
c) 性能优化：
- 复用共同的样式
- 适当使用组合（g元素）
- 避免不必要的复杂路径

请根据以上规范生成SVG代码，注意整体的美观性、专业性和清晰度。具体的样式（如颜色、尺寸、字体等）可以根据实际需求灵活调整，但要遵循上述核心原则。

请按照我的要求画一个{DIAGRAM_DESCRIPTION}
```

## Purpose
This prompt guides AI models to generate SVG code for professional swimlane diagrams that visualize processes and workflows across different departments, roles, or systems. It provides comprehensive specifications to ensure the resulting diagram is clear, visually appealing, and follows best practices in diagram design.

## Example Usage
```
请创建一个SVG格式的泳道图(Swimlane Diagram)，需要满足以下规范：
[... entire prompt above ...]
请按照我的要求画一个电子商务订单处理流程，包含客户、订单系统、支付系统、仓库四个泳道
```

## Sample Response
The AI will respond with SVG code that creates a swimlane diagram following all the specified requirements, including proper layout, connection points, visual hierarchy, and best practices for code organization.

## Notes
- Replace `{DIAGRAM_DESCRIPTION}` with your specific diagram needs
- For complex diagrams, consider providing additional details about:
  - The specific entities/swimlanes required
  - Key process steps in each lane
  - Important decision points
  - Critical connections between lanes
- The prompt is in Chinese but can be translated to other languages as needed 