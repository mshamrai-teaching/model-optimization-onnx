# Computer Vision Course Assignment: Model Optimization with ONNX

## Overview

Welcome to the Model Optimization assignment for the Computer Vision course! In this assignment, you will use ONNX to optimize and quantize a model you previously trained for Classification, Object Detection, or Semantic Segmentation. The goal is to evaluate the performance of your model before and after optimization on both CPU and GPU, using speed, compression, and accuracy metrics.

### Getting Started

1. **Prepare your pre-trained model:**
   - Ensure you have a pre-trained model for Classification, Object Detection, or Semantic Segmentation that you have trained previously.

2. **Clone this repository to your local machine:**
     ```bash
     git clone https://github.com/mshamrai-teaching/model-optimization-onnx-*your-name*
     ```
3. **Navigate to the project directory:**
      ```bash
       cd model-optimization-onnx-*your-name*
      ```

### Guidelines

* Model Optimization:
  * Export your pre-trained model to the ONNX format.
  * Use ONNX Runtime for optimization and quantization of your model.

* Evaluation:
  * Evaluate your model's performance before and after optimization on both CPU and GPU.
  * Measure speed (inference time) multiple times and report the results in the mean ± std format.
  * Assess the model compression by comparing the file sizes before and after optimization.
  * Evaluate the accuracy of your model.

* Tools and Libraries:
  *  Utilize ONNX Runtime for optimization and quantization processes.
  *  Employ libraries like NumPy, PyTorch, TensorFlow, or any other relevant tools for model evaluation and metric calculations.

### Hints

* Model Export:
  * Use framework-specific functions to export your model to ONNX. For example, use `torch.onnx` for PyTorch models.

* Optimization Techniques:
  * Explore ONNX Runtime's optimization features, including graph optimizations and quantization.
  * Consider applying both static and dynamic quantization techniques to observe their impact on performance.

* Speed Evaluation:
  * Perform inference multiple times to get reliable speed metrics.
  * Use tools like `timeit` to measure inference time accurately.
  * Take batch size into consideration, as it can significantly impact inference speed. Evaluate the model with different batch sizes to find the optimal configuration for both CPU and GPU. Plots are welcomed. 

### Submission

To submit your solution, commit your files to the `main` branch of the repository.

Ensure your final submission includes:
* Source code (main.py or similar) for exporting, optimizing, quantizing, and evaluating the model.
* A brief report (report.md or similar) describing the optimization techniques applied, evaluation results, and performance comparisons before and after optimization.
* Include all relevant metrics such as speed (mean ± std), compression ratios, and accuracy scores.

### Evaluation

Your solution will be evaluated based on the effectiveness of the optimization, the accuracy of the model post-optimization, and the clarity of your code and documentation. Special attention will be given to the detailed reporting of speed metrics in mean ± std format.

Best of luck with your assignment! If you encounter any difficulties or have questions, don't hesitate to ask for assistance.
