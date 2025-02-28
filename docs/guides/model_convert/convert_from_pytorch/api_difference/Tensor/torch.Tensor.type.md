## [torch 参数更多]torch.Tensor.type

### [torch.Tensor.type](https://pytorch.org/docs/1.13/generated/torch.Tensor.type.html#torch.Tensor.type)

```python
torch.Tensor.type(dtype=None, non_blocking=False, **kwargs)
```

### [paddle.Tensor.astype](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/Tensor_cn.html#astype-dtype)

```python
paddle.Tensor.astype(dtype)
```

其中 PyTorch 相比 Paddle 支持更多其他参数，具体如下：

### 参数映射

| PyTorch      | PaddlePaddle | 备注                                                         |
| ------------ | ------------ | ------------------------------------------------------------ |
| dtype        | dtype        | 转换后的 dtype。                                             |
| non_blocking | -            | 控制 cpu 和 gpu 数据的异步复制，Paddle 无此参数，暂无转写方式。 |
