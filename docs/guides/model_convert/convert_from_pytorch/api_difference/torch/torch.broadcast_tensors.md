## [ 输入参数类型不一致 ]torch.broadcast_tensors

### [torch.broadcast_tensors](https://pytorch.org/docs/stable/generated/torch.broadcast_tensors.html?highlight=broadcast_tensors#torch.broadcast_tensors)

```python
torch.broadcast_tensors(*tensors)
```

### [paddle.broadcast_tensors](https://www.paddlepaddle.org.cn/documentation/docs/zh/develop/api/paddle/broadcast_tensors_cn.html#broadcast-tensors)

```python
paddle.broadcast_tensors(input,
                         name=None)
```

两者功能一致但参数类型不一致，具体如下：
### 参数映射

| PyTorch       | PaddlePaddle | 备注                                                   |
| ------------- | ------------ | ------------------------------------------------------ |
| <font color='red'> *tensors </font>      | <font color='red'> input </font>      | 一组输入 Tensor ， PyTorch 参数 tensors 为可变参, Paddle 参数 inputs 为 list(Tensor) 或 tuple(Tensor) 的形式。   |


### 转写示例
#### *tensors: 一组输入 Tensor
```python
# PyTorch 写法
torch.broadcast_tensors(x, y)

# Paddle 写法
paddle.broadcast_tensors([x, y])
```