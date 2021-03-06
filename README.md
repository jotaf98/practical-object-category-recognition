# Object category recognition practical (CNN version)

> A computer vision practical by the Oxford Visual Geometry group,
> authored by Andrea Vedaldi and Andrew Zisserman.

Start from `doc/instructions.html`.

> This practical is related to the older
> `practical-category-recognition` which uses hand-crafted features
> (SIFT, Fisher Vectors, VLAD, etc.), but is based on CNN features
> instead.

Package contents
----------------

The package contains three exercises:

* `exercise1.m`: learn and test an image classifier on benchmark data
* `exercise2.m`: learn your own classifier

The practical is based on [VLFeat](http://www.vlfeat.org) and
[MatConvNet](http://www.vlfeat.org/matconvnet). This package contains
the following MATLAB functions:

* `standardizeImage.m`: Rescale an image to a standard size.
* `displayRankedImagelist.m`: Visualize a subset of a ranked list of images.
* `displaySaliencyMap.m`: Display a classifier saliency map.
* `encodeImage.m`: Encode an image using CNN features.
* `getImageSet.m`: Scan a directory for images.
* `loadEncoder.m`: Load a CNN-based encoder.
* `trainLinearSVM.m`: Learn a linear support vector machine.

Appendix: Installing from scratch
---------------------------------

1. From Bash, run `./extras/download.sh`. This will download the
   PASCAL VOC data and extract a subset of it.
2. From MATLAB, run `addpath extras ; preprocess.m`. This will download VLFeat
   and MatConvNet and precompute the data for the practical.

Changes
-------

* *2017a* - Upgrades MatConvNet and other small fixes.
* *2015b* - First version.

License
-------

    Copyright (c) 2015 Andrea Vedaldi and Andrew Zisserman.

    Permission is hereby granted, free of charge, to any person
    obtaining a copy of this software and associated documentation
    files (the "Software"), to deal in the Software without
    restriction, including without limitation the rights to use, copy,
    modify, merge, publish, distribute, sublicense, and/or sell copies
    of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be
    included in all copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
    EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
    MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
    NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
    HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
    WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
    DEALINGS IN THE SOFTWARE.
