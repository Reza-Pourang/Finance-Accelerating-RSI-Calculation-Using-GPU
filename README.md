# Accelerating RSI Calculation Using GPU

## Project Overview
This project demonstrates how GPU acceleration can significantly optimize the calculation of the Relative Strength Index (RSI), a key technical indicator used in financial trading. By leveraging GPU parallelism, it investigates the computational speedup achievable compared to traditional CPU processing, particularly for large datasets and real-time applications.

## Key Objectives
- Accelerate RSI calculations using GPU-based parallel processing.
- Benchmark performance differences between CPU and GPU implementations.
- Evaluate the scalability and efficiency of GPU acceleration for financial analytics.

## Features
- **Data Source**: Historical Forex data from [forexsb.com](https://forexsb.com/historical-forex-data).
- **GPU Library**: CuPy for Python (v12.2).
- **Environment**: Google Colab.
- **Performance Metrics**: Computation time for RSI across varying periods and dataset sizes.

## Methodology
1. **Data Preparation**: Import and preprocess historical Forex data (EURUSD, GBPUSD, USDCAD).
2. **RSI Calculation on CPU**: Implemented RSI computation using Python and pandas.
3. **GPU Acceleration**: Used CuPy to parallelize calculations.
4. **Benchmarking**: Measured execution times for both CPU and GPU implementations.
5. **Optimization**: Applied batch processing to maximize GPU utilization.

## Key Results
- GPU processing outperformed CPU by an average factor of **3.5x** for large datasets.
- Batch processing enhanced scalability and efficiency on the GPU.
- RSI values from GPU matched CPU results, ensuring accuracy.

## Data Sources
- Historical Forex data (1, 5, 15, 30-minute intervals):
  - EURUSD, GBPUSD, USDCAD
  - Provided by [forexsb.com](https://forexsb.com/historical-forex-data)

## Requirements
- Python 3.x
- Libraries: `pandas`, `numpy`, `cupy`
- Google Colab or a local environment with a CUDA-compatible GPU.
