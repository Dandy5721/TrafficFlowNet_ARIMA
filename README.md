- ARIMA_PEMS04.py
- ARIMA_PEMS07.py
- ARIMA_PEMS04.py
- 


**Refer to** # UCTB (Urban Computing Tool Box)

 [![Python](https://img.shields.io/badge/python-3.6%7C3.7-blue)]() [![PyPI](https://img.shields.io/badge/pypi%20package-v0.3.5-sucess)](https://pypi.org/project/UCTB/) [![https://img.shields.io/badge/license-MIT-green](https://img.shields.io/badge/license-MIT-green)]() [![Documentation](https://img.shields.io/badge/api-reference-blue.svg)](https://uctb.github.io/UCTB)

------


## Prediction Models

Currently, the ST prediction model package supports the following models: (This toolbox is constructed based on some open-source repos. We appreciate these awesome implements. [See more details](https://uctb.github.io/UCTB/md_file/predictive_tool.html#)). 

|  Model  |   Data Format   |   Spatial Modeling Technique   |Graph Type|Temporal Modeling Technique|Temporal Knowledge|Module|
| :--: | :--: | :--: |:--:|:--:|:--:|:--:|
|   ARIMA   |   Both   |   N/A   |N/A|SARIMA|Closeness|``UCTB.model.ARIMA``|
|   HM   |   Both   |   N/A   |N/A|N/A|Closeness|``UCTB.model.HM``|
|   HMM   |   Both   |   N/A   |N/A|HMM|Closeness|``UCTB.model.HMM``|
|   XGBoost   |   Both   |   N/A   |N/A|XGBoost|Closeness|``UCTB.model.XGBoost``|
|   DeepST [[SIGSPATIAL 2016]](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/09/DeepST-SIGSPATIAL2016.pdf)  |   Grid   |   CNN   |N/A|CNN|Closeness, Period, Trend|``UCTB.model.DeepST``|
|   ST-ResNet [[AAAI 2017]](https://arxiv.org/pdf/1610.00081.pdf)  |   Grid   |   CNN   |N/A|CNN|Closeness, Period, Trend|``UCTB.model.ST_ResNet``|
|   DCRNN [[ICLR 2018]](https://arxiv.org/pdf/1707.01926.pdf) |   Node   |   GNN   |**Prior** (Sensor Network)|RNN|Closeness|``UCTB.model.DCRNN``|
|   GeoMAN [[IJCAI 2018]](https://www.ijcai.org/proceedings/2018/0476.pdf) |   Node   |   Attention   |**Prior** (Sensor Networks)|Attention+LSTM|Closeness|``UCTB.model.GeoMAN``|
|   STGCN [[IJCAI 2018]](https://www.ijcai.org/proceedings/2018/0505.pdf) |   Node   |   GNN   |**Prior** (Traffic Network)|Gated CNN|Closeness|``UCTB.model.STGCN``|
|   GraphWaveNet [[IJCAI 2019]](https://www.ijcai.org/proceedings/2019/0264.pdf)  |   Node   |   GNN   |**Prior** (Sensor Network) + **Adaptive**|TCN|Closeness|``UCTB.model.GraphWaveNet``|
|   ASTGCN [[AAAI 2019]](https://ojs.aaai.org/index.php/AAAI/article/view/3881) |   Node   |   GNN+Attention   |**Prior** (Traffic Network)|Attention|Closeness, Period, Trend|``UCTB.model.ASTGCN``|
|  ST-MGCN [[AAAI 2019]](https://ojs.aaai.org/index.php/AAAI/article/view/4247) |   Node   |   GNN   |**Prior** (Neighborhood, Functional similarity, Transportation connectivity)|CGRNN|Closeness|``UCTB.model.ST_MGCN``|
|   GMAN [[AAAI 2020]](https://ojs.aaai.org/index.php/AAAI/article/view/5477/5333) |   Node   |   Attention   |**Prior** (Road Network)|Attention|Closeness|``UCTB.model.GMAN``|
|   STSGCN [[AAAI 2020]](https://ojs.aaai.org/index.php/AAAI/article/view/5438) |   Node   |   GNN+Attention   |**Prior** (Spatial Network)|Attention|Closeness|``UCTB.model.STSGCN``|
|  AGCRN [[NeurIPS 2020]](https://proceedings.neurips.cc/paper/2020/file/ce1aad92b939420fc17005e5461e6f48-Paper.pdf) |   Node   |   GNN   |**Adaptive**|RNN|Closeness|``UCTB.model.AGCRN``|
|  MTGNN [[KDD 2020]](https://dl.acm.org/doi/abs/10.1145/3394486.3403118) |   Node   |   GNN   |**Adaptive**|TCN|Closeness|``UCTB.model.MTGNN``|
|   STMeta [[TKDE 2021]](https://arxiv.org/abs/2009.09379)  |   Node   |   GNN   |**Prior** (Proximity, Functionality, Interaction/Same-line)|LSTM/RNN|Closeness, Period, Trend|``UCTB.model.STMeta``|
