# -Runoff-Prediction-Model-CSVWCRBA-
The coupled model integrating secondary decomposition, deep learning algorithms, and intelligent optimization algorithms
Installation Guide
This model requires Python 3.9 and the following packages:

PyTorch 1.12.0+cu113 (with CUDA 11.3 configured for NVIDIA GPU acceleration)
numpy 1.23.5, matplotlib 3.7.1, pandas 1.5.3

We recommend managing dependencies via a virtual environment (e.g., conda or venv). Steps:

Create and activate a Python 3.9 virtual environment.
Install the PyTorch GPU version (supporting CUDA 11.3) and other required packages.
Verify GPU availability: Ensure PyTorch detects your graphics card and can invoke CUDA.
Usage Instructions
1. Run the Pre-Optimized Model
After installation, execute the main prediction script in your Python environment, specifying the input data path (e.g., monthly runoff data for the Longmen Hydrological Station). The model will automatically load pre-trained parameters and generate predictions.
2. Parameter Optimization (Optional)
The model includes modules for parameter optimization using the Sparrow Search Algorithm (SSA) and Whale Optimization Algorithm (WOA). Due to complex computations, the optimization process is time-consuming—adjust configurations based on your hardware capabilities.

Pre-optimized code: Ready-to-use code without the optimization process is provided for quick predictions.
Original optimization code: Separate SSA and WOA scripts are available for researchers to reproduce the optimization workflow, but note that runtime may range from hours to days.
Important Notes
GPU Configuration: Ensure CUDA Toolkit 11.3 and compatible graphics drivers are installed to leverage GPU acceleration for training and prediction.
Memory Management: If encountering memory issues, adjust batch sizes in the configuration file or use smaller datasets for testing.


The source code is released under the Apache License 2.0, allowing free use, modification, and distribution for both academic and commercial purposes.
