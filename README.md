# Image Captioning with Attention Network

This repo contains the implementation of [Show, Attend and Tell: Neural Image Caption Generation with Visual Attention](http://arxiv.org/abs/1502.03044) which introduces attention mechanism for Image caption generator.

## Introduction

 - The input is an image, and the output is a sentence describing the content of the image.
 - It first uses a convolutional neural network to extract a feature vector of the input image, and then uses a LSTM recurrent neural network to decode this feature vector into a natural language sentence.
 - A soft attention mechanism is incorporated to improve the quality of the caption.

## Examples
<div class="display: inline-block; float: left;">
 <img src="/Example/4.jpg" width="436px" alt="Example 1">
 <img src="/Example/3.jpg" width="436px" alt="Example 2">
</div>
</br></br>
<div class="display: inline-block; float: left;">
 <img src="/Example/5.jpg" height="450px" width="436px" alt="Example 3">
 <img src="/Example/6.jpg" height="450px" width="436px" alt="Example 4">
</div>

## References

Borrowed most of the code from 
 - Author's theano code: https://github.com/kelvinxu/arctic-captions 
 - Another tensorflow implementation: https://github.com/jazzsaxmafia/show_attend_and_tell.tensorflow
 - Another tensorflow implementation: https://github.com/yunjey/show-attend-and-tell
    
## Related Work

 1) [Show and Tell](https://arxiv.org/abs/1411.4555) extracted high level image feature and fed to the LSTM to generate the captions.
 2) [Show, Attend and Tell](https://arxiv.org/abs/1502.03044) added attention mechanism to the caption generating process.
 3) [Stacked Attention Networks](https://arxiv.org/abs/1511.02274) runs multiple iterations to infer the answer progressively, which helps in capturing fine-grained information from the question.
 
## Architecture

## Dependencies

This code is written in python
 - Python 2.7
 - A relatively recent version of [NumPy](http://www.numpy.org/)
 - Tensorflow

