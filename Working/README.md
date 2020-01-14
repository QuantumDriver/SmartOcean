### Baseline1
- 参考[jt120](https://github.com/jt120/tianchi_ship_2019)的代码,新增的y_max_over_x_min特征提升了不少F1-Score
- 数据探索显示了三种渔船的一些工作特色
- 对X和Y做了比较多的特征工程
- 快速形成一个baseline

### Baseline2
- 省去数据探索和加载,直接读取baseline1形成的h5文件
- 对于x和y做了更多的特征工程,如y/x,x/y
- 尝试两个lightgbm模型进行融合,发现效果不佳
- 用一个lightgbm去做10折交叉验证,效果再次提升

### Baseline3
- 更多特征
- 调参
- 更多模型融合
