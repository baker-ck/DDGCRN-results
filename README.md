# Decomposition Dynamic Graph Convolutional Recurrent Neural Network (DDGCRN) results
This folder contains trained DDGCRN models on traffic data (PEMSD3, PEMSD4, PEMSD7, PEMSD8) and test results.

### Implementation notes
We used the publicly available DDGCRN (https://github.com/wengwenchao123/DDGCRN) codebase as our training framework. No changes were made to model architectures, loss functions or optimisation measures.

### Repo structure
```
DDGCRN-results/
├── README.md
├── pre-trained-model/
├── pre-trained-model-results/
│   └─── PEMSD3/
│        └─── model.pth
│   └─── PEMSD4/
│        └─── model.pth
│   └─── PEMSD7(M)/
│        └─── model.pth
│   └─── PEMSD7/
│        └─── model.pth
│   └─── PEMSD8/
│        └─── model.pth
├── re-trained/
├── re-trained-model-results/
│   └─── PEMSD3/
│        └─── model.pth
│   └─── PEMSD4/
│        └─── model.pth
│   └─── PEMSD7(M)/
│        └─── model.pth
│   └─── PEMSD7/
│        └─── model.pth
│   └─── PEMSD8/
│        └─── model.pth
└── requirements.txt
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
| Average Horizon      |      |    |     |

#### Pre-trained Model: DDGCRN (Weng et al., 2023)
- Dataset: PEMSD4
- Horizons: 12
- Criterion: validation loss

|    | MAE       | RMSE      | MAPE      |
| ---------- | --------- | --------- | --------- |
| Average Horizon      |      |    |     |


#### Pre-trained Model: DDGCRN (Weng et al., 2023)
- Dataset: PEMSD7(M)
- Horizons: 12
- Criterion: validation loss

|    | MAE       | RMSE      | MAPE      |
| ---------- | --------- | --------- | --------- |
| Average Horizon      |      |    |     |


#### Pre-trained Model: DDGCRN (Weng et al., 2023)
- Dataset: PEMSD7
- Horizons: 12
- Criterion: validation loss

|    | MAE       | RMSE      | MAPE      |
| ---------- | --------- | --------- | --------- |
| Average Horizon      |      |    |     |

#### Pre-trained Model: DDGCRN (Weng et al., 2023)
- Dataset: PEMSD8
- Horizons: 12
- Criterion: validation loss

|    | MAE       | RMSE      | MAPE      |
| ---------- | --------- | --------- | --------- |
| Average Horizon      |      |    |     |

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
