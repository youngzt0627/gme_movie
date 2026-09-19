# GME Movie

一个基于 TensorFlow 1.x 的电影推荐实验项目，包含基础 DNN 训练和带邻居历史信息的预热/元学习流程。

## 主要文件

- `gme_movie/base_dnn.py`：训练基础推荐模型
- `gme_movie/warm_up_dnn_base.py`：运行预热与元学习实验
- `gme_movie/config_*.py`：模型及数据配置
- `gme_movie/ctr_funcs.py`：数据读取与公共函数

## 运行

准备 TFRecord 数据并放入代码所需的 `data/`、`data_with_hist/` 目录，然后执行：

```bash
cd gme_movie
python base_dnn.py
python warm_up_dnn_base.py
```

训练数据和模型文件未包含在仓库中。

