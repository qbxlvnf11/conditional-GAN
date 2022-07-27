Description
=============

#### - Conditional GAN (CGAN)

<img src="https://user-images.githubusercontent.com/52263269/181246936-54cf9e93-1ab2-4a1a-9896-8f5c241903d8.png" width="60%"></img>

- Conditional version of generative adversarial nets
  - In an unconditioned generative model, there is no control on modes of the data being generated.
  - In the Conditional GAN (CGAN), the generator learns to generate a fake sample with a specific condition or characteristics (such as a label associated with an image or more detailed tag) rather than a generic sample from unknown noise distribution. 
  - Simply feeding the data y, and conditioning both the generator and discriminator
- Loss

<img src="https://user-images.githubusercontent.com/52263269/181247747-39457171-bb0a-446f-bf51-92f9403d3025.png" width="80%"></img>

Contents
=============

#### - [Generating Fashion MNIST Image with CGAN](https://github.com/qbxlvnf11/conditional-GAN/blob/main/conditional-GAN-generating-fashion-mnist.ipynb)
- Generator
  - Input: z (100 dimension), Output: generated image
  - FC [256, 512, 1024]
- Discriminator: FC-base
  - Input: image (generated or real), Output: fake/real
- Adversarial learning: refer to generator_train_step(), discriminator_train_step()

Dataset
=============

#### - Fashion MNIST

https://www.kaggle.com/datasets/zalando-research/fashionmnist

References
=============

#### - CGAN code

https://www.kaggle.com/code/arturlacerda/pytorch-conditional-gan/notebook

#### - CGAN Paper
```
@article{CGAN,
  title={Conditional Generative Adversarial Nets},
  author={Mehdi Mirza, Simon Osindero},
  journal = {arXiv},
  year={2014}
}
```

Author
=============

#### - LinkedIn: https://www.linkedin.com/in/taeyong-kong-016bb2154

#### - Blog URL: https://blog.naver.com/qbxlvnf11

#### - Email: qbxlvnf11@google.com, qbxlvnf11@naver.com
