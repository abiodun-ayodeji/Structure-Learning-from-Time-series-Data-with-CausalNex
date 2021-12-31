# Structure-Learning-from-Time-series-Data-with-CausalNex

## Time series data structure learning with NOTEARS and DYNOTEARS 


### Introduction

You must have heard the phrase "correlation is not causation". The phrase explains one of the issues with the conventional deep learning approach especially for long sequence time series dataset - the learned pattern (correlation) may be spurious. 

To address the spurious correlation issue, a number of approaches, such as causal machine learning, and graph neural network are being proposed. However, learning the graph (structure) in time series datasets is a non-trivial task. This repository demonstrates how to use a public library - [CausalNex](https://causalnex.readthedocs.io/en/latest/) - with NOTEARS and [DYNOTEARS](https://arxiv.org/abs/2002.00498) to learn the dependencies (graph/structure) in sensors that define aircraft degradation history.

Learning the connections (structures) between time-varying parameters, and using the learned connections to build a deep learning model would improve the performance of the resulting model.  The learned structure can be used to build a graph neural network, with better predictive performance than the conventional correlation-based deep learning model. The CausalNex API also flexible, as it enables the integration of domain knowledge (i.e.nodes and edges can be added or removed from the extracted graph)

### Data

The dataset is the degradation data that defines turbofan engine run-to-failure  history, provided by NASA.

### Usage

See the notebook

### Links

[1] Pamfil et al. 2020: DYNOTEARS: Structure Learning from Time-Series Data. ArXiv, 2020

[2] CausalNex [API](https://causalnex.readthedocs.io/en/latest/causalnex.html)
