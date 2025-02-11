## [ 仅 paddle 参数更多 ] torch.ShortTensor

### [torch.ShortTensor](https://pytorch.org/docs/stable/tensors.html)

```python
torch.ShortTensor(data)
```

### [paddle.to_tensor](https://www.paddlepaddle.org.cn/documentation/docs/zh/develop/api/paddle/to_tensor_cn.html#to-tensor)

```python
paddle.to_tensor(data, dtype=paddle.int16, place="cpu")
```

其中 Paddle 比 PyTorch 支持更多参数，具体如下：

### 参数映射

| PyTorch | PaddlePaddle | 备注                                                      |
| ------- | ------------ | --------------------------------------------------------- |
| -       | dtype        | Tensor 的数据类型，Paddle 为 paddle.int16，需要进行转写。 |
| -       | place        | Tensor 的设备，Paddle 为 cpu，需要进行转写。              |

### 转写示例

#### Paddle 参数转写

```python
# PyTorch 写法:
torch.ShortTensor([1, 2])

# Paddle 写法:
paddle.to_tensor([1, 2], place="cpu", dtype=paddle.int16)
```
