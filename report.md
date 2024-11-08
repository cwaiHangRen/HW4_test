## HW4 Image Generation with GAN
> 崔灏睿 2022010907 计28-经22
### 1. 模型训练结果
使用的超参数如下：
```
```
**latent_dim=hidden_dim=16**
|D_G_z1|D_G_z2|D_x__|
|:----:|:----:|:----:|
| | | |

|Loss_G|Loss_D|Sample|
|:----:|:----:|:----:|
| | | |

**latent_dim=16,hidden_dim=100**
|D_G_z1|D_G_z2|D_x__|
|:----:|:----:|:----:|
| | | |
|Loss_G|Loss_D|Sample|
|:----:|:----:|:----:|
| | | |

**latent_dim=100,hidden_dim=16**
|D_G_z1|D_G_z2|D_x__|
|:----:|:----:|:----:|
| | | |

|Loss_G|Loss_D|Sample|
|:----:|:----:|:----:|
| | | |

**latent_dim=hidden_dim=100**
|D_G_z1|D_G_z2|D_x__|
|:----:|:----:|:----:|
| | | |

|Loss_G|Loss_D|Sample|
|:----:|:----:|:----:|
| | | |

### 2. FID score评估结果
|latent_dim\hidden_dim| 16 | 32 | 64 | 100 |
|:-------------------:|:--:|:--:|:--:|:---:|
| 16                  |73.8| | |54.0 |
| 32                  |    | | | |
| 64                  |    | | | |
| 100                 |71.9| | |35.2|
### 3. latent_dim & hidden_dim 对模型的影响
### 4. 更换 DCGAN 实现
#### 4.1 用 LeakyReLU 替换 ReLU
#### 4.2 删除BN层
#### 4.3 模型比较
### 5. 纳什均衡