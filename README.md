# Website Benchmarking Guide

This guide describes how to benchmark the performance of your website hosted at `http://167.71.165.62:8501/` using two popular tools: Apache Benchmark (`ab`) and `wrk`.

## Prerequisites

Make sure you have the following tools installed on your Ubuntu system:

1. **Apache Benchmark (`ab`)**
2. **wrk**

### Installing Apache Benchmark

To install Apache Benchmark, run the following command:

```bash
sudo apt-get install apache2-utils
ab -n 1000 -c 100 http://167.71.165.62:8501/
```

OR

```bash
sudo apt-get install wrk
wrk -t8 -c400 -d30s http://167.71.165.62:8501/
```
