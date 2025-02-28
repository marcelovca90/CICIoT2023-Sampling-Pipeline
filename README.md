# A Sample-Based, Multi-Stage Machine Learning Pipeline for Scalable IoT Threat Detection

> Marcelo V. C. Aragão, Tiago de M. Pereira, Felipe A. P. de Figueiredo, and Samuel B. Mafra

_Abstract_: The rapid growth of IoT devices demands scalable and efficient threat detection solutions. This paper introduces a sample-based, multi-stage machine learning (ML) pipeline for IoT threat detection using the CICIoT2023 dataset, integrating feature selection, data balancing, and hyperparameter optimization to improve detection accuracy while reducing the computational overhead associated with training. We evaluate LightGBM, XGBoost, and XGBoostRF across binary, multiclass, and fine-grained tasks, showing that XGBoost with 10% sampling achieves the best trade-off between accuracy and efficiency. Compared to prior methods, our approach eliminates GPU dependence, maintains low latency, and preserves state-of-the-art performance while enabling scalable training for high generalization capacity. Additionally, we provide model selection guidelines based on dataset complexity and computational constraints. The results show that training with a sample-based approach enables effective threat detection on large datasets, producing models that generalize well to diverse IoT attack scenarios, thus ensuring practical applicability in real-world deployments.

### Setup

```
conda create -n "CICIoT2023-Sampling-Pipeline" python=3.11
conda activate CICIoT2023-Sampling-Pipeline
pip install -r requirements.txt
```

### Execution

```
jupyter lab
- For a single experiment: pipeline_code.ipynb
- For multiple experiments: pipeline_runner.ipynb
```
