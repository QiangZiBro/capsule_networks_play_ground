# How to define a capsule?
As we know, capsules are produced by primary capsule layer, each output capsule is defined as  8 dimension vector on every pixel position of the feature image. So we get 6x6 size of image, meaning that we shall have 6x6 vectors from one **channel**. Note the channel definition here, actually it is 8 dimension feature map as a result of convolution operation. In the example of original paper, the output capsule dimension is 32.

- What's the difference of implementation between 8 32 channel convolution and 1 256 convolution and then split it to 32 equal part?
Actually, two implementations are the same, and they all can be found on open source project.    - [capsule-utils](https://github.com/gchochla/capsules-utils/blob/master/examples/capsnet.ipynb) use 1 256 convolution and get 98.78% accuracy.



