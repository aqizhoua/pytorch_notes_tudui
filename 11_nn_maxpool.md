- maxpool
  - 最大池化，指取一个卷积核范围内的最大值,下采样
  - 同理，平均池化，指一个卷积核范围内的平均值
  - 参数：只需设置kernel_size和ceil_mode，其他保持默认即可
    - ceil_mode默认为False
    - ceil_mode为True代表向上去整，即当剩余尺寸小于kernel_size大小时，仍然进行处理
  - input输入要reshape为4维，4个维度分别为batch_size,channel,H,W
  - input输入要为浮点型，不能为整型