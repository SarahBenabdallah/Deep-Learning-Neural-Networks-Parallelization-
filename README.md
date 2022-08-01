End of year project: DEEP LEARNING PARALLELIZATION BY NEURAL NETWORKS FOR BIOLOGICAL AND MEDICAL ANALYSIS

Biological and medical databases have considerably grown since many years. A base request that only took a few minutes can now take days. At the same time, the bioinformatics research community has developed, and specialized laboratories have been established around the world. Using many data science methods to study these databases, training Convolutional Neural Networks (CNN) has been one of the most computationally intensive task whose parallelization has become critical in order to complete the training in an acceptable time.

However, there are two obstacles to developing a scalable parallel CNN in a distributedmemory computing environment. One is the high degree of data dependency exhibited in the model parameters across every two adjacent mini-batches and the other is the large amount of data to be transferred across the communication channel. Here, we present a parallelization strategy that maximizes the overlap of inter-process communication with the computation.

The overlapping is achieved by using a thread per compute node to initiate communication after the gradients are available. The output data of backpropagation stage is
generated at each model layer, and the communication for the data can run concurrently with the computation of other layers.
To study the effectiveness of the overlapping and its impact on the scalability, we studied various model architectures and distributed training methods.
