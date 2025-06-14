Description:

What I learned:
Python:

Math:

AI:
- tanh saturation
  - occurs for very large positive or negative inputs
  - tanh output approaches -1 or 1
  - tanh graph flattens out as it approaches -1 or 1
  - effect: vanishing gradients
- dead neurons
- batch normalization
  - used to control statistics of activations in neural net
  - usually placed after layers that have multiplication
  - how it works
    - calculates mean and std of activations
    - centers batch to be unit gaussian
    - offsets and scales batch by learned bias and gain
    - also keeps track of running mean and std to be used during inference
