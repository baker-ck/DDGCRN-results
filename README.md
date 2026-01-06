# Decomposition Dynamic Graph Convolutional Recurrent Neural Network (DDGCRN) results
This folder contains trained DDGCRN models on traffic data (PEMSD3, PEMSD4, PEMSD7, PEMSD8) and test results.

### Implementation notes
We used the publicly available DDGCRN (https://github.com/wengwenchao123/DDGCRN) codebase as our training framework. No changes were made to model architectures, loss functions or optimisation measures.

### Repo structure
```
DDGCRN-results/
├── README.md
├── pre-trained-models/
│   └─── PEMSD3.pth
│   └─── PEMSD4.pth
│   └─── PEMSD7.pth
│   └─── PEMSD7(M).pth
│   └─── PEMSD8.pth
├── testing/
│   └─── PEMSD3_run.log
│   └─── PEMSD4_run.log
│   └─── PEMSD7_run.log
│   └─── PEMSD7(M)_run.log
│   └─── PEMSD8_run.log
└── environment.yaml
```

### Environment
- Python:  3.6.5
- PyTorch: 1.8.1
- Device: CUDA (NVIDIA GTX 1060, 3GB)
- Conda environment exported in `environment.yaml`

### Results
#### Pre-trained Model: DDGCRN (Weng et al., 2023)
- Dataset: PEMSD3
- Horizons: 12
- Criterion: validation loss

|    | MAE       | RMSE      | MAPE      |
| ---------- | --------- | --------- | --------- |
| Average Horizon      | 14.5219     | 25.1095   | 0.1449    |

#### Pre-trained Model: DDGCRN (Weng et al., 2023)
- Dataset: PEMSD4
- Horizons: 12
- Criterion: validation loss

|    | MAE       | RMSE      | MAPE      |
| ---------- | --------- | --------- | --------- |
| Average Horizon      |  18.5068    |  30.7219  |  0.1235   |


#### Pre-trained Model: DDGCRN (Weng et al., 2023)
- Dataset: PEMSD7(M)
- Horizons: 12
- Criterion: validation loss

|    | MAE       | RMSE      | MAPE      |
| ---------- | --------- | --------- | --------- |
| Average Horizon      |  2.5939    | 5.3171   |  0.0654   |


#### Pre-trained Model: DDGCRN (Weng et al., 2023)
- Dataset: PEMSD7
- Horizons: 12
- Criterion: validation loss

|    | MAE       | RMSE      | MAPE      |
| ---------- | --------- | --------- | --------- |
| Average Horizon      |  19.6810    | 33.4056   | 0.0823    |

#### Pre-trained Model: DDGCRN (Weng et al., 2023)
- Dataset: PEMSD8
- Horizons: 12
- Criterion: validation loss

|    | MAE       | RMSE      | MAPE      |
| ---------- | --------- | --------- | --------- |
| Average Horizon      |  14.3187    |  23.7136  |  0.0938   |

### References

The implementation for DDGCRN (Weng et al.) is based on the Pattern Recognition 2023 paper “A decomposition dynamic graph convolutional recurrent network for traffic forecasting” (https://www.sciencedirect.com/science/article/abs/pii/S0031320323003710), with the following citation:

```bibtex
@article{weng2023decomposition,
  title={A decomposition dynamic graph convolutional recurrent network for traffic forecasting},
  author={Weng, Wenchao and Fan, Jin and Wu, Huifeng and Hu, Yujie and Tian, Hao and Zhu, Fu and Wu, Jia},
  journal={Pattern Recognition},
  volume={142},
  pages={109670},
  year={2023},
  publisher={Elsevier}
}
```
