## [ torch 参数更多 ] torch.hub.list

### [torch.hub.list](https://pytorch.org/docs/stable/hub.html?highlight=hub+list#torch.hub.list)

```python
torch.hub.list(github,
                force_reload=False,
                skip_validation=False,
                trust_repo=None)
```

### [paddle.hub.list](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/hub/list_cn.html)

```python
paddle.hub.list(repo_dir,
                source='github',
                force_reload=False)
```


其中，PyTorch 相比 Paddle 支持更多其他参数，具体如下：

### 参数映射
| PyTorch       | PaddlePaddle | 备注                                                   |
| ------------- | ------------ | ------------------------------------------------------ |
| github        | repo_dir      |repo 地址，支持 git 地址形式和 local 地址，仅参数名不同。|
| force_reload   | force_reload |指定是否强制拉取，默认值: False。             |
| skip_validation| -            |检查由 github 参数指定的分支或提交是否属于存储库所有者，Paddle 无此参数，一般对网络训练结果影响不大，可直接删除。|
| trust_repo     | -            |在 v1.14 中被移除；Paddle 无此参数，一般对网络训练结果影响不大，可直接删除。|
| -              |source        |指定 repo 托管的位置，Pytorch 无此参数，Paddle 保持默认即可|
