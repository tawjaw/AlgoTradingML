# AlgoTradingML
## Comparison of Different Algorithmic Trading Strategies on Tesla Stock Price

### Tawfiq Jawhar
<b>Machine Learning (COMP-652 and ECSE-608)<br>
Fall 2018<br>
McGill University <br><br>
Instructors:<br>
Audrey Durand<br>
Riashat Islam <br></b>


## Notebooks

[1- Trading Environment and Buy and Hold Benchmark](https://github.com/tawjaw/AlgoTradingML/blob/master/1-%20Environment%20and%20Buy%20and%20Hold%20Benchmark.ipynb)

[2- Extracting Data for Learning](https://github.com/tawjaw/AlgoTradingML/blob/master/2-%20Extracting%20Data%20for%20Learning.ipynb)

[3- Exploring TSLA](https://github.com/tawjaw/AlgoTradingML/blob/master/3-%20Exploring%20TSLA.ipynb)

[4- Regime Detection with GMM](https://github.com/tawjaw/AlgoTradingML/blob/master/4-%20Regime%20Detection%20with%20GMM.ipynb)

[5- SMA Optimization](https://github.com/tawjaw/AlgoTradingML/blob/master/5-%20SMA%20Optimization.ipynb)

[6- SE-MA Optimization](https://github.com/tawjaw/AlgoTradingML/blob/master/6-%20SE-MA%20Optimization.ipynb)

[7- MA with GMM Risk Manager](https://github.com/tawjaw/AlgoTradingML/blob/master/7-%20MA%20with%20GMM%20Risk%20Manager.ipynb)

[8- Price Movement Classifiers](https://github.com/tawjaw/AlgoTradingML/blob/master/8-%20Price%20Movement%20Classification.ipynb)

## Installation
The trading environment will be used for backtesting is [Zipline](https://github.com/quantopian/zipline) which is an open source Python algorithmic trading library. Zipline is used as the backtesting and live-trading engine powering [Quantopian](https://www.quantopian.com/home).

To simplify the installation I created a docker image on DockerHub. The docker image is based on Dockerfile found in zipline repo.

To pull the docker image:

```
docker pull tawjaw/ziplineml
```
To run the docker use:
```
docker run -v /path/to/your/notebooks:/projects -v ~/.zipline:/root/.zipline -p 8888:8888/tcp --name zipline -it docker pull tawjaw/ziplineml:v1
```
The default password for Jupyter is `jupyter`.

