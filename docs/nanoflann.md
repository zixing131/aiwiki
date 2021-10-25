---
Title | nanoflann
-- | --
Create Date | `2021-10-22T16:05:39Z`
Update Date | `2021-10-22T16:05:39Z`
Edit link | [here](https://github.com/junxnone/aiwiki/issues/123)

---
# Reference
- [nanoflann - Github](https://github.com/jlblancoc/nanoflann)
- [Docs](http://jlblancoc.github.io/nanoflann/)

# Brief
- 基于 FLANN
- 相对 [Original FLANN](https://github.com/junxnone/tech-io/issues/991) 50% 性能提升
- C++11
- header-only - `include/nanoflann.hpp`
- Content
  - Building KD-trees
  - Querying closest neighbors
    - KnnSearch() - **最近的 N 个点**
    - RadiusSearch() - **半径 R 内的点**
    - radiusSearchCustomCallback()
## Pipeline
- 1 Define kd-tree
  - 1.1 Set Input
- 2 Search
  - 2.1 knnSearch()
  - 2.2 radiusSearch()
- 3 Outputs
  - 3.1 N 
  - 3.2 index
  - 3.3 distance

## Distance Metrics

Type | Distance | Description
-- | -- | --
R^N Euclidean spaces | L1 | Manhattan
x+ | L2 | squared Euclidean norm, favoring SSE2 optimization
x+ | L2_Simple | squared Euclidean norm, for low-dimensionality data sets like point clouds
SO(2) 2D rotational group | metric_SO2 | Absolute angular diference
SO(3) 3D rotational group | metric_SO3 | Inner product between quaternions

# UseCase
