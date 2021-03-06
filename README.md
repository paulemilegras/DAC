# Data Aggregation with Clustering (DAC)

Companion Github repository to Data Aggregation and Demand Prediction



## Install the dependencies
```
pip install -r requirements.txt
```

## Structure of the repository:

Simulation: apply DAC on a generated dataset

Real_Data: apply DAC on a real dataset we provide or on your own dataset


## About the algorithm
We propose a practical method -referred to as the Data Aggregatino with Clustering (DAC) algorithm - that balances the tradeoff between data aggregation adn model flexibility. The Dac allows us to predict demand while optimally identifying the features that should be estimated at the (i) item, (ii) cluster, and (iii) aggregated levels. We analytically show that the DAC yields a consistent esimate along with improved asymptotic properties relative to the tradional ordinary least squares method that treats different items in a decentralized fashion. Using both simulated and real data, we illustrate the improvement in prediction accuracy obtained by the DAC relative to several common benchmarks. Interestingly, the DAC not only has theoretical and practical advantages, it also helps retailers discover useful managerial insights. See full details in the [article](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3411653) 



