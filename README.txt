What I learned:
Python:
- torch:
  - torch.no_grad(): disables gradient tracking

Math:
- standard deviation: how spread out data is from mean
- normal/Gaussian distribution: probability distribution symmetric about mean
  - unit normal distribution: special case when mean = 0 and std = 1

AI:
- tanh saturation
  - occurs for very large positive or negative inputs
  - tanh output approaches -1 or 1 --> graph flattens out
    - effect: vanishing gradients
- dead neurons: always output the same value no matter the input
  - effect: do not contribute to learning process
- batch normalization
  - used to control statistics of activations in neural net
  - usually placed after layers that have multiplication
  - how it works
    - calculates mean and std of activations
    - centers batch to be unit Gaussian
    - offsets and scales batch by learned bias and gain
    - also keeps track of running mean and std to be used during inference
- using graphs to diagnose issues in a complex neural net
