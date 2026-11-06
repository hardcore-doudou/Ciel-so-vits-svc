# 训练记录 / Training record

检查日期 / Inspection date: 2026-11-06

## 已核实 / Verified

| 字段 / Field | 记录 / Record |
| --- | --- |
| Checkpoint | G_31200.pth; 627,905,309 bytes |
| Saved step / epoch | 31,200 / 459, confirmed by training log |
| Configuration | config.json, inspected locally; not distributed |
| Speaker mapping | Ciel: 0 |
| Sample rate | 44,100 Hz |
| Encoder / SSL dimension | vec768l12 / 768 |
| Vocoder | nsf-hifigan |
| Automatic F0 prediction | Enabled in configuration |
| Volume embedding | Disabled |
| Batch size | 4 |
| Learning rate (configured initial value) | 0.0001 |
| FP16 training | fp16_run: false |
| Checkpoint type | Log reports model and optimizer state saved |

日志在保存后继续记录至 Epoch 468，最后显示的训练步数为 31,800；本次检查到的最新权重仍为 31,200 步，不能把后续日志步数当作该权重的保存步数。

The log continues through epoch 468 and reports step 31,800 after the checkpoint save. The latest checkpoint observed remains step 31,200; later log entries do not establish a later saved model.

## 待验证 / Pending

- Exact framework revision; checkpoint structure and configuration compatibility.
- SHA-256 checksums and reproducible inference test.
- Dataset duration, clip count, source permissions and distribution terms.
- Hardware, total training time and evaluation of checkpoint quality.
- Independently authorized audio demonstrations.

配置可读及日志对应不等于已验证推理兼容性。训练损失不能替代试听评估。
Readable configuration and corresponding logs do not establish inference compatibility. Training loss alone does not establish perceptual quality.
