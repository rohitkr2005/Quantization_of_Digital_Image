# Image Quantization Visualizer

An interactive web-based visualization tool demonstrating how bit depth controls the number of intensity levels (shades) in digital image processing. 

Experience the live demo here: [Insert your GitHub Pages link here]

## 📌 Overview

In digital image processing, quantization is the process of mapping a continuous range of pixel intensities to a finite set of discrete values. This tool provides a hands-on way to explore how decreasing the bit depth reduces the available shades of gray and color, leading to visible banding or "false contouring."

## ✨ Features

* **Interactive Bit Depth Selection**: Toggle between 1-bit and 8-bit depths to instantly see the impact on image quality.
* **Multi-Channel Visualization**: Real-time rendering of quantization effects across Grayscale, Red, Green, and Blue channels.
* **Dynamic Mathematical Breakdown**: Automatically calculates and displays the step sizes, input ranges, and output values based on the selected bit depth.
* **Zero Dependencies**: Built entirely with vanilla HTML, CSS, and JavaScript.

## 🧮 The Mathematics

The number of distinct intensity levels ($L$) a pixel can have is determined by the bit depth ($n$):

$$L = 2^n$$

For example, an 8-bit image provides $2^8 = 256$ distinct shades, creating smooth gradients. A 3-bit image only provides $2^3 = 8$ shades. 

To map a standard 8-bit pixel value ($0$ to $255$) down to a lower bit depth, the visualizer calculates a step size:

$$\text{Step Size} = \frac{256}{L}$$

The input pixel intensity ($I$) is then mapped to a specific level index, which determines its final quantized output value.


## 🤝 Contributing

Feel free to fork this project, submit pull requests, or open an issue if you find a bug or have a feature request.
