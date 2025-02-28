## [torch 参数更多]torch.Tensor.round

### [torch.Tensor.round](https://pytorch.org/docs/1.13/generated/torch.Tensor.round.html#torch.Tensor.round)

```python
torch.Tensor.round(decimals=0)
```

### [paddle.Tensor.round](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/Tensor_cn.html#round-name-none)

```python
paddle.Tensor.round(name=None)
```

其中 PyTorch 相比 Paddle 支持更多其他参数，具体如下：

### 参数映射
| PyTorch  | PaddlePaddle | 备注 |
| -------- | ------- | ------- |
| decimals | -       | 舍入小数位数 |

### 转写示例
#### decimals：要舍入到的小数位数
```python
# Pytorch 写法
torch.tensor([3.345, 5.774]).round(decimals=2)

# Paddle 写法
(paddle.to_tensor([3.345, 5.774]) * 1e2).round() / 1e2

# 注：Paddle 可使用 10 的 decimals 次方来实现
```
