# gpuhook
 You can use this so to hook the cuMemGetInfo CUDA function. And the gpu memory will be the env GPU_MEMORY 's value

```
[GCC 5.4.0 20160609] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import tensorflow as tf
>>> sess =tf.Session()
2019-03-22 13:09:02.797279: I tensorflow/core/platform/cpu_feature_guard.cc:140] Your CPU supports instructions that this TensorFlow binary was not compiled to use: SSE4.1 SSE4.2 AVX AVX2 FMA
env GPU_MEMORY is not set use default value 2GB
hacking gpu memory from env GPU_MEMORY by lovejoy. mem=<2147483648>
2019-03-22 13:09:02.970249: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1344] Found device 0 with properties:
name: Tesla K20c major: 3 minor: 5 memoryClockRate(GHz): 0.7055
pciBusID: 0000:02:00.0
totalMemory: 2.00GiB freeMemory: 1.00GiB
2019-03-22 13:09:02.970316: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1423] Adding visible gpu devices: 0
2019-03-22 13:09:03.269970: I tensorflow/core/common_runtime/gpu/gpu_device.cc:911] Device interconnect StreamExecutor with strength 1 edge matrix:
2019-03-22 13:09:03.270021: I tensorflow/core/common_runtime/gpu/gpu_device.cc:917]      0
2019-03-22 13:09:03.270035: I tensorflow/core/common_runtime/gpu/gpu_device.cc:930] 0:   N
env GPU_MEMORY is not set use default value 2GB
hacking gpu memory from env GPU_MEMORY by lovejoy. mem=<2147483648>
2019-03-22 13:09:03.270220: I tensorflow/core/common_runtime/gpu/gpu_device.cc:1041] Created TensorFlow device (/job:localhost/replica:0/task:0/device:GPU:0 with 799 MB memory) -> physical GPU (device: 0, name: Tesla K20c, pci bus id: 0000:02:00.0, compute capability: 3.5)
```
