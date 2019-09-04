# Tensorflow Handbook for TPU on Google Cloud


![TPU on Google Cloud](docs/images/tensorflow-tpu.png)

This repository is the [TPU Chapter](https://tf.wiki/zh/appendix/tpu.html) for [简单粗暴TensorFlow | A Concise Handbook of TensorFlow](https://tf.wiki)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/huan/tensorflow-handbook-tpu/blob/master/tensorflow-handbook-tpu-example.ipynb)

Book Chapter: TPU for Tensorflow - <https://huan.github.io/tensorflow-handbook-tpu/>

![TPU on Google Cloud](docs/images/tpu-pod.jpg)

## INSTALL

### Moung Google Storage Bucket as Local Directory

Install `gcsfuse` to mount Googl Cloud Storage Bucket.

> <https://github.com/GoogleCloudPlatform/gcsfuse/blob/master/docs/installing.md#ubuntu-and-debian-latest-releases>

```sh
export GCSFUSE_REPO=gcsfuse-`lsb_release -c -s`
echo "deb http://packages.cloud.google.com/apt $GCSFUSE_REPO main" | sudo tee /etc/apt/sources.list.d/gcsfuse.list
curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -

sudo apt-get update
sudo apt-get install gcsfuse
```

## Links

- [Reference models and tools for Cloud TPUs](https://github.com/tensorflow/tpu)
- [Tensorflow Official Document: Distribute Strategy - TPUStrategy](https://www.tensorflow.org/guide/distribute_strategy#tpustrategy)
- [Tensorflow Official Guide: Using TPUs](https://www.tensorflow.org/guide/using_tpu)
- [Distributed Training in TensorFlow: Strategy](https://www.tensorflow.org/guide/distribute_strategy#using_tfdistributestrategy_with_custom_training_loops)
- [Distributed training in TensorFlow: Keras](https://www.tensorflow.org/tutorials/distribute/keras)
- [Running MNIST on Cloud TPU](https://cloud.google.com/tpu/docs/tutorials/mnist)

## Author

[Huan](https://github.com/huan) [(李卓桓)](https://linkedin.com/in/zixia) \<zixia@zixia.net\>

<a href="http://stackoverflow.com/users/1123955/huan">
  <img src="http://stackoverflow.com/users/flair/1123955.png" width="208" height="58" alt="profile for zixia at Stack Overflow, Q&amp;A for professional and enthusiast programmers" title="profile for zixia at Stack Overflow, Q&amp;A for professional and enthusiast programmers">
</a>

## Copyright & License

- Code & Docs © 2019 - now Huan LI \<zixia@zixia.net\>
- Code released under the Apache-2.0 License
- Docs released under Creative Commons
