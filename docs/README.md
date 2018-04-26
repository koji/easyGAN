---
home: true
---

## What is GAN?

GAN stands for Generative adversarial network.  
Generative adversarial networks (GANs) are a class of artificial intelligence algorithms used in unsupervised machine learning, implemented by a system of two neural networks contesting with each other in a zero-sum game framework. They were introduced by Ian Goodfellow et al. in 2014.[1] This technique can generate photographs that look at least superficially authentic to human observers, having many realistic characteristics (though in tests people can tell real from generated in many cases).[2][from wikipedia](https://en.wikipedia.org/wiki/Generative_adversarial_network)

## What is easyGAN?

easyGAN is a python module which offers an opportunity to try DCGAN easily.

## Install

[pypi-easyGAN](https://pypi.org/project/easygan/)

```bash
$ pip install easygan
```

## How to Use

easyGAN has two features. One is to collect images from the internet.  
The other is to run DCGAN with images collected by easygan command.

### Collect Images

```bash
$ easygan --search "google" --keyword "puppy" --folder "puppies"

--search: search engine(currently easygan only suppoprts google image search. will support flickr soon.)

--keyword: search query You can put anything you want.
If you want to use multiple keywords, you need to input the following.

--keyword "NYC food"

--folder: This will be used as a folder name which easygan saves images.
```

### Run DCGAN

This phase will take much time if you don't have GPU.  
If you run this command successfully, easygan will create the folder, "results" the place you run easygan.

```bash
$ easygan --folder "puppies" --batch 55

--folder: This must be the folder name which has images
If you collect images by yourself and save them in a specific folder, you need to input the name.

--batch: This is batch size.
```

## ToDo
- [ ] Flickr API
- [ ] Bing Image search API
- [ ] DuckDuckGo Image search
- [ ] Suppoert ffmpeg for making a video file


### Example

<gifs></gifs>
