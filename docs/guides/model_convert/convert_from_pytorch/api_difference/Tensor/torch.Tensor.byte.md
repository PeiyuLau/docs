## [ torch 参数更多 ] torch.Tensor.byte

### [torch.Tensor.byte](https://pytorch.org/docs/1.13/generated/torch.Tensor.byte.html#torch.Tensor.byte)

```python
torch.Tensor.byte(memory_format=torch.preserve_format)
```

### [paddle.Tensor.astype](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/Tensor_cn.html#astype-dtype)

```python
paddle.Tensor.astype('uint8')
```

其中 Pytorch 相比 Paddle 支持更多其他参数，具体如下：

### 参数映射

| PyTorch       | PaddlePaddle | 备注                                                                                |
| ------------- | ------------ | ----------------------------------------------------------------------------------- |
| memory_format | -            | 表示内存格式， Paddle 无此参数，一般对网络训练结果影响不大，可直接删除。    |

### 转写示例

```python
# torch 写法
x = torch.tensor([0, 1, 2, 3])
y = x.byte()

# paddle 写法
x = paddle.to_tensor([0, 1, 2, 3])
y = x.astype('uint8')
```
