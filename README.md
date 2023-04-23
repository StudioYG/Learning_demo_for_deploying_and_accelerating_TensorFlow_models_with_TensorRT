# Learning demo for deploying and accelerating TensorFlow models with TensorRT

TensorRT provides three types of precision mode (FP32, FP16, and INT8) to optimize deep learning models, therefore, accelerating the inference process. The steps of INT8 are different from FP32 and FP16. Before model quantization, INT8 requires to additionally build a calibration dataset to cover the expected distribution of data scenarios. In this demo, ConvNeXtTiny (a large model variant) is used to evaluate the inference performance accelerated by different precision modes. 

# Inference performance comparison
 precision mode      | Average inference time per 50 steps (ms)     | Throughput (images/s)   
 -------- | :-----------:  | :-----------: 
 FP32     | 126.1     | 127       
 FP16     | 124.3     | 129       
 INT8     | 119.2     | 134
