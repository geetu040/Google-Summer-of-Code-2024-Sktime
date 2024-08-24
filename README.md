<img src="assets/gsoc-sktime-banner.png" alt="Google Summer of Code 2024 - Sktime Project Banner" width="100%">
<hr>

# ⭐️ About Project

| **Program**        | **Google Summer of Code, 2024**                                                                                                                             |
| :----------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Organisation**   | [Sktime](https://summerofcode.withgoogle.com/programs/2024/organizations/sktime): A unified framework for ML with time series                               |
| **Project**        | Sktime integration with deep learning backends - pytorch and huggingface - [Dashboard](https://summerofcode.withgoogle.com/programs/2024/projects/f5FggiB7) |
| **Mentors**        | [Franz Király](https://github.com/fkiraly) - [Benedikt Heidrich](https://github.com/benHeid) - [Anirban Ray](https://github.com/yarnabrina)                 |
| **Project Length** | 350 hours                                                                                                                                                   |

### Overview

I worked with sktime as a Google Summer of Code student during the period late May to August 2024. This post is created to summarise the work I’ve done over this period as the work product submission required to be submitted at the end of GSoC.

Sktime is a library for time series analysis in Python. It provides a unified interface for multiple time series learning tasks like classification, regression, clustering, annotation, and forecasting.

My project was focused on implementing and interfacing deep learning models in sktime leveraging PyTorch and Hugging Face.

### Topics

`Data Science` - `AI` - `Time Series` - `Toolbox Frameworks` - `Machine Learning` - `Deep Learning`

### Technologies

`Python` - `GitHub` - `Pytorch` - `Huggingface` - `Scikit-Learn`

### Outcomes

- Enhanced skills in PyTorch and Hugging Face.
- Improved Python coding practices, focusing on writing efficient, high-quality code.
- Gained experience in test-driven development and designing optimal code solutions.
- Acquired knowledge of machine learning and deep learning techniques for time-series data analysis.
- Familiarized with time-series-related libraries and packages.
- Gained insights into the life cycle, development, and maintenance of a Python package through hands-on experience with sktime.
- Enhanced experience in open-source project contributions.
- Strengthened Git and GitHub skills.
- Improved communication with mentors and collaboration on complex design decisions.

### Challenges

- Initially, managing time was challenging, as it was my first experience working on a project of this scale.
- Maintaining consistency with daily stand-ups and weekly mentoring sessions was difficult at first.
- Understanding and making changes to a large, complex codebase was particularly tough.
- I had to dive deeper into certain libraries to implement features effectively, requiring more in-depth knowledge than I initially had.
- I discovered that designing solutions was more challenging than implementing them, leading me to focus more on efficient design strategies before execution.

# 🎯 Contributions

## Pull Requests

These contributions primarily involve the implementation of new algorithms and the enhancement and fixing of existing ones.

| **Pull Request**                                    | **Status** | **Title**                                                                            | **Related Issue**                                     |
| :-------------------------------------------------- | :--------- | :----------------------------------------------------------------------------------- | ----------------------------------------------------- |
| [#6928](https://github.com/sktime/sktime/pull/6928) | Draft      | [ENH] Global Forecast API for BaseDeepNetworkPyTorch based interfaces                | [#6836](https://github.com/sktime/sktime/issues/6836) |
| [#6842](https://github.com/sktime/sktime/pull/6842) | Open       | [ENH] Implements Autoregressive Wrapper                                              | [#6802](https://github.com/sktime/sktime/issues/6802) |
| [#6571](https://github.com/sktime/sktime/pull/6571) | Open       | [ENH] interface to TimesFM Forecaster                                                | [#6408](https://github.com/sktime/sktime/issues/6408) |
| [#6791](https://github.com/sktime/sktime/pull/6791) | Merged     | [ENH] Pytorch Classifier & de-novo implementation of Transformer                     | [#6786](https://github.com/sktime/sktime/issues/6786) |
| [#6712](https://github.com/sktime/sktime/pull/6712) | Merged     | [ENH] Interface to TinyTimeMixer foundation model                                    | [#6698](https://github.com/sktime/sktime/issues/6698) |
| [#6202](https://github.com/sktime/sktime/pull/6202) | Merged     | [ENH] de-novo implementation of LTSFTransformer based on cure-lab research code base | [#4939](https://github.com/sktime/sktime/issues/4939) |
| [#6457](https://github.com/sktime/sktime/pull/6457) | Merged     | [ENH] Extend HFTransformersForecaster for PEFT methods                               | [#6435](https://github.com/sktime/sktime/issues/6435) |
| [#6321](https://github.com/sktime/sktime/pull/6321) | Merged     | [BUG] fixes failing test in neuralforecast auto freq, amid pandas freq deprecations  |                                                       |
| [#6237](https://github.com/sktime/sktime/pull/6237) | Merged     | [ENH] Update doc and behavior of freq="auto" in neuralforecast                       |                                                       |
| [#6367](https://github.com/sktime/sktime/pull/6367) | Merged     | [MNT] final change cycle (0.30.0) for renaming cINNForecaster to CINNForecaster      | [#6120](https://github.com/sktime/sktime/issues/6120) |
| [#6238](https://github.com/sktime/sktime/pull/6238) | Merged     | [MNT] change cycle (0.29.0) for renaming cINNForecaster to CINNForecaster            | [#6120](https://github.com/sktime/sktime/issues/6120) |

In addition to this, these PRs were submitted during the application review period.

| **Pull Request**                                    | **Status** | **Title**                                                                            | **Related Issue**                                     |
| :-------------------------------------------------- | :--------- | :----------------------------------------------------------------------------------- | ----------------------------------------------------- |
| [#6121](https://github.com/sktime/sktime/pull/6121) | Merged     | [MNT] initialize change cycle (0.28.0) for renaming cINNForecaster to CINNForecaster | [#6120](https://github.com/sktime/sktime/issues/6120) |
| [#6039](https://github.com/sktime/sktime/pull/6039) | Merged     | [ENH] NeuralForecastRNN should auto-detect freq                                      |                                                       |
| [#6088](https://github.com/sktime/sktime/pull/6088) | Merged     | [MNT] create build tool to check invalid backticks                                   |                                                       |
| [#6023](https://github.com/sktime/sktime/pull/6023) | Merged     | [DOC] Fix invalid use of single-grave in docstrings                                  |                                                       |
| [#6116](https://github.com/sktime/sktime/pull/6116) | Merged     | [ENH] Adds MSTL import statement in detrend                                          | [#6085](https://github.com/sktime/sktime/issues/6085) |
| [#6059](https://github.com/sktime/sktime/pull/6059) | Merged     | [ENH] Examples for YtoX transformer docstring                                        |                                                       |

## Walk Through

Here, I will walk through some of the major contributions, from the above pull requests, where I added estimators to sktime.

To see the working and inference of these estimators, please refer to [code.ipynb](./code.ipynb).

### ⚡ MVTSTransformerClassifier

- **Title:** [ENH] PyTorch Classifier & De-Novo Implementation of Transformer
- **Status:** Merged
- **Pull Request:** [#6791](https://github.com/sktime/sktime/pull/6791)
- **Related Issue:** [#6786](https://github.com/sktime/sktime/issues/6786)
- **Research Paper:** [A Transformer-based Framework for Multivariate Time Series Representation Learning](https://dl.acm.org/doi/abs/10.1145/3447548.3467401)
- **Official Code:** [gzerveas/mvts_transformer](https://github.com/gzerveas/mvts_transformer)
- **Sktime Source Code:** [sktime/classification/deep_learning/mvts_transformer.py](https://github.com/sktime/sktime/blob/main/sktime/classification/deep_learning/mvts_transformer.py)

This pull request introduces the `MVTSTransformerClassifier`, based on the paper "A Transformer-based Framework for Multivariate Time Series Representation Learning," applying it to classification and regression.

I implemented the [BaseDeepClassifierPytorch](https://github.com/sktime/sktime/pull/6791/files#diff-bbe6571ca91b7ba8297d9c19de41b7a86f201533bac9d307ea3a99781726841c) class as a foundation for PyTorch-based classifiers. Then, I used the [TSTransformerEncoderClassiregressor](https://github.com/sktime/sktime/pull/6791/files#diff-8eef014681dea4cdf5c555aadf8e08ab1535f57de6b332ed7fa0e972272a609a) to build the PyTorch network. Finally, I created the [MVTSTransformerClassifier](https://github.com/sktime/sktime/pull/6791/files#diff-44b50f069a3c5c1dbf87bec02ac01fc5658391a07590f4bccf92cf6a2b5ec214) class to integrate the network with the base class.

This process enhanced my understanding of transformer architecture.

The estimator can be loaded into sktime using the following code:

```python
from sktime.classification.deep_learning import MVTSTransformerClassifier

model = MVTSTransformerClassifier(
    d_model=256,
    n_heads=4,
    num_layers=4,
    dim_feedforward=128,
    dropout=0.1,
    pos_encoding="fixed",
    activation="relu",
    norm="BatchNorm",
    freeze=False,
)
```

For more details on how the estimator works, please refer to [code.ipynb](./code.ipynb).

### ⚡ TinyTimeMixer

- **Title:** [ENH] Interface to TinyTimeMixer Foundation Model
- **Status:** Merged
- **Pull Request:** [#6712](https://github.com/sktime/sktime/pull/6712)
- **Related Issue:** [#6698](https://github.com/sktime/sktime/issues/6698)
- **Research Paper:** [Tiny Time Mixers (TTMs): Fast Pre-trained Models for Enhanced Zero/Few-Shot Forecasting of Multivariate Time Series](https://www.researchgate.net/profile/Vijay-Ekambaram/publication/381111250_Tiny_Time_Mixers_TTMs_Fast_Pre-trained_Models_for_Enhanced_ZeroFew-Shot_Forecasting_of_Multivariate_Time_Series/links/665d8c5d0b0d2845747de5f5/Tiny-Time-Mixers-TTMs-Fast-Pre-trained-Models-for-Enhanced-Zero-Few-Shot-Forecasting-of-Multivariate-Time-Series.pdf)
- **Official Code:** [ibm-granite/granite-tsfm](https://github.com/ibm-granite/granite-tsfm)
- **Sktime Source Code:** [sktime/forecasting/ttm.py](https://github.com/sktime/sktime/blob/main/sktime/forecasting/ttm.py)

TinyTimeMixer (TTM) is a compact, pre-trained model for time-series forecasting, developed and open-sourced by IBM Research.

In this PR, I integrated TTM into the sktime framework by forking the official code into the [sktime/libs/granite_ttm](https://github.com/sktime/sktime/pull/6712/files#diff-b3059a73c53cb90d9ba1a01f34ded57098aa285d85d170320011e39474fc4ca9) directory, as the source package was not available on PyPI.

Next, I developed an interface for the estimator within the [TinyTimeMixerForecaster](https://github.com/sktime/sktime/pull/6712/files#diff-0a25dac16832f47a85e6d03327d4270510efa529cf0e42e1fc71786dde192711) class.

Throughout this implementation, I gained valuable experience in creating custom Hugging Face models and configurations, loading and modifying weights, altering architecture, and training newly initialized weights.

The estimator can now be loaded into sktime using the following code:

```python
from sktime.forecasting.ttm import TinyTimeMixerForecaster

model = TinyTimeMixerForecaster(
    model_path="ibm/TTM",
    revision="main",
    validation_split=0.2,
    config=None,
    training_args=None,
    compute_metrics=None,
    callbacks=None,
    broadcasting=False,
    use_source_package=False,
)
```

For further details on how the estimator functions, please refer to [code.ipynb](./code.ipynb).

### ⚡ LTSFTransformer

- **Title:** [ENH] De-Novo Implementation of LTSFTransformer Based on Cure-Lab Research Codebase
- **Status:** Merged
- **Pull Request:** [#6202](https://github.com/sktime/sktime/pull/6202)
- **Related Issue:** [#4939](https://github.com/sktime/sktime/issues/4939)
- **Research Paper:** [Are Transformers Effective for Time Series Forecasting?](https://ojs.aaai.org/index.php/AAAI/article/view/26317)
- **Official Code:** [cure-lab/LTSF-Linear](https://github.com/cure-lab/LTSF-Linear)
- **Sktime Source Code:** [sktime/forecasting/ltsf.py](https://github.com/sktime/sktime/blob/main/sktime/forecasting/ltsf.py)

This pull request introduces the `LTSFTransformer`, an implementation based on the paper "Are Transformers Effective for Time Series Forecasting?" which explores the application of transformer architecture to time series forecasting.

To begin the implementation, I structured the transformer architecture in the [sktime/networks/ltsf/layers](https://github.com/sktime/sktime/pull/6202/files#diff-0a18272d47c22fc6c495216fa5c757ee77153b9ddbc04daa00895a00ffa472a1) directory, along with the PyTorch dataset class [PytorchFormerDataset](https://github.com/sktime/sktime/pull/6202/files#diff-af8d474dbf509d241fd02bcc6071c7758ca194d93d3a9f1e3f25ebc8db1809ec).

Next, I developed the [LTSFTransformerNetwork](https://github.com/sktime/sktime/pull/6202/files#diff-598a15fdb2a333630aad06167788a7f9ec31eb46d4aae59687b0be38c872a7eb) interface class by leveraging the base PyTorch forecasting class, which connects to the network created in the previous step.

Throughout this implementation, I gained valuable insights into transformer architecture, particularly in applying various embeddings and encodings to temporal features in time series data.

The estimator can be loaded into sktime with the following code:

```python
from sktime.forecasting.ltsf import LTSFTransformerForecaster

model = LTSFTransformerForecaster(
    seq_len=30,
    context_len=15,
    pred_len=15,
    num_epochs=50,
    batch_size=8,
    in_channels=1,
    individual=False,
    criterion=None,
    criterion_kwargs=None,
    optimizer=None,
    optimizer_kwargs=None,
    lr=0.002,
    position_encoding=True,
    temporal_encoding=True,
    temporal_encoding_type="embed",  # linear, embed, fixed-embed
    d_model=32,
    n_heads=1,
    d_ff=64,
    e_layers=1,
    d_layers=1,
    factor=1,
    dropout=0.1,
    activation="relu",
    freq="M",
)
```

For further details on how the estimator functions, please refer to [code.ipynb](./code.ipynb).

### ⚡ TimesFM

- **Title:** [ENH] Interface to TimesFM Forecaster
- **Status:** Open
- **Pull Request:** [#6571](https://github.com/sktime/sktime/pull/6571)
- **Related Issue:** [#6408](https://github.com/sktime/sktime/issues/6408)
- **Research Paper:** [A Decoder-Only Foundation Model for Time-Series Forecasting](https://arxiv.org/abs/2310.10688)
- **Official Code:** [google-research/timesfm](https://github.com/google-research/timesfm)

TimesFM (Time Series Foundation Model) is a pre-trained model developed by Google Research, designed specifically for time-series forecasting.

While integrating this model into sktime, I encountered new libraries and packages. Due to dependency conflicts with the package available on PyPI, I forked the code to [sktime/libs/timesfm](https://github.com/sktime/sktime/pull/6571/files#diff-b64af953ed44337ca037cf681922b13563eff8208ea0fee96518d4f8b7d114b0).

I then created an interface for the model within the [TimesFMForecaster](https://github.com/sktime/sktime/pull/6571/files#diff-862938919a3ce54a64d3ff4f207d897e90e1d729b6c6cd52f2d9cfd9377808cc) class.

Throughout this implementation, I gained hands-on experience with foundation models and explored their capabilities.

This Pull Request is still in progress, but when merged, you can load the estimator into sktime using the following code:

```python
from sktime.forecasting.timesfm_forecaster import TimesFMForecaster

forecaster = TimesFMForecaster(
    context_len=64,
    horizon_len=32,
)
```

For more details on how the estimator functions, please refer to [code.ipynb](./code.ipynb).

### ⚡ PEFT for HFTransformersForecaster

- **Title:** [ENH] Extend HFTransformersForecaster for PEFT Methods
- **Status:** Merged
- **Pull Request:** [#6457](https://github.com/sktime/sktime/pull/6457)
- **Related Issue:** [#6435](https://github.com/sktime/sktime/issues/6435)

The `HFTransformersForecaster` in sktime allows users to load and fine-tune pre-trained models from Hugging Face. In this PR, I extended the `HFTransformersForecaster` to support Parameter-Efficient Fine-Tuning (PEFT) methods, enabling more efficient fine-tuning of large pre-trained models using customized configurations.

Through this implementation, I gained a deeper understanding of various PEFT techniques and how they can enhance the fine-tuning process for large-scale models.

You can now load the estimator in sktime with a PEFT configuration using the following code:

```python
from sktime.forecasting.hf_transformers_forecaster import HFTransformersForecaster
from peft import LoraConfig

forecaster = HFTransformersForecaster(
    model_path="huggingface/autoformer-tourism-monthly",
    fit_strategy="peft",
    training_args={
        "num_train_epochs": 20,
        "output_dir": "test_output",
        "per_device_train_batch_size": 32,
    },
    config={
        "lags_sequence": [1, 2, 3],
        "context_length": 2,
        "prediction_length": 4,
        "use_cpu": True,
        "label_length": 2,
    },
    peft_config=LoraConfig(
        r=8,
        lora_alpha=32,
        target_modules=["q_proj", "v_proj"],
        lora_dropout=0.01,
    )
)
```

For more details on how the estimator works, please refer to [code.ipynb](./code.ipynb).

### ⚡ AutoregressiveWrapper

- **Title:** [ENH] Implement Autoregressive Wrapper
- **Status:** Open
- **Pull Request:** [#6842](https://github.com/sktime/sktime/pull/6842)
- **Related Issue:** [#6802](https://github.com/sktime/sktime/issues/6802)

In sktime, some global forecasters require the forecasting horizon to be specified during the fitting process, limiting their ability to predict on different horizons afterward. This pull request introduces the `AutoregressiveWrapper`, which wraps around these forecasters, allowing them to forecast on varying horizons while fitting on a fixed horizon that is generated internally.

During this implementation, I deepened my understanding of pandas indexes, particularly in handling multi-indexes. By the end of the process, I was able to create efficient and reliable code.

This PR is still in progress, but once merged, you can load a forecaster and apply the `AutoregressiveWrapper` using the following code:

```python
from sktime.forecasting.pytorchforecasting import PytorchForecastingNBeats
from sktime.forecasting.compose import AutoRegressiveWrapper

forecaster = PytorchForecastingNBeats(trainer_params={
    "max_epochs": 20,
})

wrapper = AutoRegressiveWrapper(
    forecaster=forecaster,
    horizon_length=5,
    aggregate_method=np.mean,
)
```

For more details on how the estimator works, please refer to [code.ipynb](./code.ipynb).

### ⚡ Global Forecasting for PyTorch Models

- **Title:** [ENH] Global Forecast API for BaseDeepNetworkPyTorch-Based Interfaces
- **Status:** Draft
- **Pull Request:** [#6928](https://github.com/sktime/sktime/pull/6928)
- **Related Issue:** [#6836](https://github.com/sktime/sktime/issues/6836)

This PR enhances the `BaseDeepNetworkPyTorch` class to support global forecasting, enabling models like `CINNForecaster` and the `LTSF` family to operate as global forecasters.

Although still a work in progress, once merged, these models can be loaded and trained on hierarchical data, similar to other global forecasters in the sktime framework.

## Future Work

Some relevant future work:
- There is a list of foundation models, expected to be integrated in sktime - [#6177](https://github.com/sktime/sktime/issues/6177)
- Some estimators are required to be extended for global forecasting interface - [#6836](https://github.com/sktime/sktime/issues/6836)
- Enhancements are expected around the pytorch adapter for forecasting - [#6641](https://github.com/sktime/sktime/issues/6641)
- Improvements are also planned with the global forecasting interface - [#6997](https://github.com/sktime/sktime/issues/6997)
- Enabling PEFT for foundation models - [#6968](https://github.com/sktime/sktime/issues/6968)

# ⭐️ Achnowledgements

I had a great experience over the summer, and although the GSoC period is coming to an end, going forward I shall continue to remain a contributor to sktime. I'm incredibly thankful to both Google and sktime for giving me this opportunity, and to the welcoming community and amazing mentors at sktime for making this experience such a memorable one. There is no doubt that I am a better coder than I was 4 months ago, and I'm eagerly looking forward to learning more in the time to come.
