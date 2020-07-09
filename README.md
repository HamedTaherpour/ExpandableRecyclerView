# ExpandableRecyclerView ![Bintray](https://img.shields.io/bintray/v/pokercc/android/ExpandableRecyclerView)
使用RecyclerView 实现的折叠列表

## 效果图

### 粘性头部:
![粘性头部](./img/stick_header.gif)


### 最后一个条目展开动画:
![最后一个条目展开](./img/last_group_expand.gif)

### GridLayoutManager:
![GridLayout](./img/grid_layout.gif)

## 支持特性:
- 流畅的展开和关闭动画
- 支持只展开一个Group
- 支持展开和关闭全部
- 支持多类型item
- 支持LinearLayoutManager和GridLayoutManager
- 支持粘性头(Sticky Header)
- 展开的状态保存和恢复(横竖屏切换时)

## 欢迎下载demo，体验效果
下载地址:https://www.pgyer.com/ExpandableRecyclerView
![ExpandableRecyclerView](./img/ExpandableRecyclerView.png)

## 如何使用:
1. 引入依赖
```implementation("pokercc.android.ExpandableRecyclerView:expandableRecyclerView:${last_version}")```

2. 配置代码
- 在布局中使用ExpandableRecyclerView
- 继承ExpandableAdapter,实现自己的adapter


注意事项:
- 使用StickyHeaderRecyclerViewContainer，GroupViewHolder.itemView请设置不透明的背景，否则会发生穿透的情况
- ExpandableRecyclerView的height需要设置为match_parent或固定大小,否则在展开和关闭时，RecyclerView的高度会发生变化导致动画的执行有问题 