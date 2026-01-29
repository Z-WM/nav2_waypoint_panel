# Nav2 路点导航插件

这是一个Rviz2插件，为navigation2路点导航设计。

## 编译安装

```bash
colcon build --symlink-install
```

## 使用流程

1.  **添加面板**：Rviz2 顶部菜单 `Panels` -> `Add New Panel` -> `Waypoint Navigation`。
2.  **添加工具**：点击顶部工具栏 **`+`** 图标，添加 **`waypoint`**。
3.  **收集路径**：使用 **`waypoint`** 工具（快捷键 **W**）在地图上点选。
4.  **执行任务**：点击面板上的 **Start Nav** 开始导航。
5.  **导入导出**：点击 **Export File** 保存当前路点序列，点击 **Load File** 加载已保存的路点。



## 接口信息

*   **目标话题**：`/waypoint` (PoseStamped)
*   **核心 Action**：`follow_waypoints` (Nav2)
*   **可视化话题**：`waypoint_markers` (MarkerArray)
