---
Title | 3D Algos ICP
-- | --
Create Date | `2021-10-13T01:21:32Z`
Update Date | `2021-10-13T01:21:32Z`
Edit link | [here](https://github.com/junxnone/aiwiki/issues/86)

---
# Reference
- [迭代最近点（Iterative Closest Point, ICP）算法介绍](https://zhuanlan.zhihu.com/p/35893884)
- [【点云精配准】Iterative Closest Point（ICP）](https://zhuanlan.zhihu.com/p/107218828)

# Brief
- ICP - `Iterative Closest Point`
- 最近邻法估计 Scene 中点对应的Model 点
- 通过最小二乘法构建目标函数，进行迭代优化
- ANN - Approximate Nearest Neighbor
- SVD


分类 | Description
-- | --
point-to-point | 原始 ICP 算法
point-to-plane | 计算源点到目标点所在面的距离
plane-to-plane | 计算面到面的距离
GICP | Generalized ICP 
NICP | Normal Iterative Closest Point
point-to-line
MBICP

# 问题推导

Name | 公式
-- | --
Model 点 | ![image](https://user-images.githubusercontent.com/2216970/117235265-fc689700-ae58-11eb-9031-f877eebde05c.png)
Scene 点 | ![image](https://user-images.githubusercontent.com/2216970/117235277-025e7800-ae59-11eb-9ea8-8f684caa12d4.png)
两组点可以通过旋转平移变换 | ![image](https://user-images.githubusercontent.com/2216970/117235297-0d190d00-ae59-11eb-9cd4-81ecfcaaf8a0.png)
最小化目标函数 | ![image](https://user-images.githubusercontent.com/2216970/117235439-481b4080-ae59-11eb-9a7d-c358d25d3eb4.png)



# UseCase

![upvoglEXX2](https://user-images.githubusercontent.com/2216970/117272623-f4771a00-ae8d-11eb-9808-28699cf10014.gif)
