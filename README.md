# STS2 地图生成可视化

这是一个单文件 GitHub Pages 页面，用于模拟和展示《Slay the Spire 2》反编译源码里的 `StandardActMap` 地图生成流程。

页面包含：

- 章节预设：Overgrowth、Underdocks、Hive、Glory
- 地图种子和随机计数器
- 多人模式房间数调整
- 倒数第 7 层宝箱替换为精英
- 第二 Boss 节点
- 剪枝修复开关
- 节点类型统计和坐标显示

主要逻辑来自本地反编译源码：

- `StandardActMap.cs`
- `MapPathPruning.cs`
- `MapPostProcessing.cs`
- `MapPoint.cs`
- `MapPointTypeCounts.cs`

说明：页面种子对应地图 RNG 的直接 seed。如果要和游戏内某一局 run seed 做完全对照，还需要接入游戏里 `RunState.Rng.Seed + "act_x_map"` 的命名派生逻辑。
