CIFAR-10 PARSER
===============

## usage
Download the CIFAR-10 [dataset](http://www.cs.toronto.edu/~kriz/cifar-10-binary.tar.gz) and unzip. Clone repository in unzipped folder and install dependencies with `npm install`. Run parser for example with `node parser.js -i ./../data_batch_1.bin -p`

## purpose
This initial code is a way to get to grips with the CIFAR-10 dataset & prepare for usage in other systems like [Torch](http://torch.ch/).

## improvements
Currently writing images to disk is blocking as the read loop waits for a callback from writing an RGB buffer to png. Can be paralleled with promises or other throttling.