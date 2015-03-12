# MLP character recognition

Trains a multi-layer perceptron (MLP) neural network to recognize arbitrary characters. The training set is automatically generated using the captcha-generator [node-captcha](http://npmjs.com/package/node-captcha), which distorts the input characters with text transformations.

The script moves each character to the center of the 256-bit (16x16) network input using a center of mass calculation to maximize success rate.

Currently the MLP has a success rate of ```~70%``` on numbers ```0-9``` and a success rate of ```~50%``` on letters ```a-z```.

Below are examples of input images from training sets generated for recognition of numbers 0-9 and letters a-z respectively.

![0-9](https://raw.github.com/mateogianolio/mlp-character-recognition/master/examples/0-9.png)

![a-z](https://raw.github.com/mateogianolio/mlp-character-recognition/master/examples/a-z.png)

## Usage

Clone this repository and make sure the ```input``` folder exists before running

```bash
$ npm install
$ node main.js
```

## Contribute

Feel free to fork and submit pull requests.