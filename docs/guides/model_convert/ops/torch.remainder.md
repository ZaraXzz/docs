## torch.remainder
### [torch.remainder](https://pytorch.org/docs/stable/generated/torch.remainder.html?highlight=remainder#torch.remainder)

```python
torch.remainder(input,
                other,
                *,
                out=None)
```

### [paddle.remainder](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/remainder_cn.html#remainder)

```python
paddle.remainder(x,
                 y,
                 name=None)
```

其中 Pytorch 相比 Paddle 支持更多其他参数，具体如下：
### 参数差异
| PyTorch       | PaddlePaddle | 备注                                                   |
| ------------- | ------------ | ------------------------------------------------------ |
| input         | x            | 被除数，Pytorch 可为 Tensor or Scalar，Paddle 仅可为 Tensor。  |
| other         | y            | 除数，Pytorch 可为 Tensor or Scalar，Paddle 仅可为 Tensor。   |
| out           | -            | 表示输出的 Tensor，PaddlePaddle 无此参数。               |


### 转写示例
#### out：指定输出
```python
# Pytorch 写法
torch.remainder([3, 5], 2, out=y)

# Paddle 写法
y = paddle.remainder([3, 5], 2)
```