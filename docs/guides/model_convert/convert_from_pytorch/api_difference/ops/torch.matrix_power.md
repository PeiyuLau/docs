## [torch 参数更多 ]torch.matrix_power
### [torch.matrix_power](https://pytorch.org/docs/1.13/generated/torch.matrix_power.html?highlight=matrix_power)
```python
torch.matrix_power(input, n, *, out=None)
```

### [paddle.linalg.matrix_power](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/linalg/matrix_power_cn.html)
```python
paddle.linalg.matrix_power(x, n, name=None)
```

其中 Pytorch 相比 Paddle 支持更多其他参数，具体如下：
### 参数映射
| PyTorch       | PaddlePaddle | 备注                                                   |
| ------------- | ------------ | ------------------------------------------------------ |
| input         | x            | 输入的 Tensor ，仅参数名不同。                             |
| n             | n            | 输入的 int ，参数完全一致。                             |
| out           | -            | 表示输出的 Tensor，PaddlePaddle 无此参数，需要进行转写。  |


### 转写示例
#### out：指定输出
```python
# Pytorch 写法
torch.matrix_power(torch.tensor([[1., 2., 3.],[1., 4., 9.],[1., 8., 27.]]), 2, out=y)

# Paddle 写法
paddle.assign(paddle.linalg.matrix_power(paddle.to_tensor([[1., 2., 3.],[1., 4., 9.],[1., 8., 27.]]), 2), y)
```
