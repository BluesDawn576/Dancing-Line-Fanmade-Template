# Dancing Line Fanmade Template

__本项目为跳舞的线自制关卡模板，还在更新中，非最终版本，请选择性使用！__

__请注意，使用本模板需要有一定的 C# 基础，不提供 C# 基础教程！__

如果您没有任何 C# 基础，您可以学习一下 C# 或者也可以在[这里](https://chinadlrs.com/developer/)选择其他模板使用

## 环境要求

- Unity 2019.3.10f1 及以上

## 可选的编辑使用的 文本编辑器 / IDE

- [Visual Studio Code](https://code.visualstudio.com/)
  - 功能丰富的文本编辑器，虽然也可以用但是个人不太推荐拿来写 C#
- [Visual Studio 2022](https://visualstudio.microsoft.com/)
  - 体验还行，但是配合 Unity 的使用体验上可能没有 Rider 舒服
- [Rider](https://www.jetbrains.com/rider/)
  - 个人推荐，配合 Unity 使用体验上很舒服，~~但是付费~~

## 一些吐槽

太喜欢写 Manager (Singleton) 了导致了到处都是 Instance 跳来跳去的不太好拓展见谅，如果需要自己拓展一些功能可能需要修改一下模板的代码

## 更新日志

### 2024/1/1 - 上传到 GitHub
- 上传到 GitHub

### 2024/1/1 - 2024010100 更新
- 修改了部分类的访问权限到 internal
- 将 ReadyUI 作为单独类便于管理
- 新增暂停界面 UI 便于返回起始状态
- 优化了 UIManager 的结构，将各种 UI 整合到 UIComponents.cs 里了

### 2024/1/2 - 2024010200 更新
- 现在会在 MainLine 加载实例时 (Awake) 自动设置 _onGround，避免会在初次开始游玩时有粒子产生 
- 增加空场景 (此空场景为 SampleScene 修改，并非重新制作) 便于制作

### 2024/1/4 - 2024010400 更新
> 不确定修改为抛物线是否会对性能产生较大的影响，可以选择改回 CubicIn + CubicOut 的形式
- 修改 ButtonAttribute 的命名空间到 DancingLineSample.Attributes 下
- 修改皇冠效果动画为抛物线 (CheckpointObject.cs)
- 新增皇冠效果动画抛物线预览
- 新增相机跟随数据预览
- 修复打包时报错的问题 (为 UnityEditor 相关引起的问题)
- 增加 AudioOffset 按钮组 (位于 Setting UI)，为下次更新准备
