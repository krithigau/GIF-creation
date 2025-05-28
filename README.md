# GIF Creator with Python

Generate an animated GIF from multiple images using Python and the `imageio.v3` library.

---

## 🌀 Overview

This project demonstrates how to combine a sequence of static images into an animated GIF using Python. The generated GIF loops infinitely with a customizable frame duration.

## 🚀 Features

- Combines multiple images into a smooth animation  
- Customizable frame duration and loop settings  
- Simple and lightweight implementation  

## 🛠 Requirements

- Python 3.x  
- `imageio` (version 3.x)

Install dependencies using:

```bash
pip install imageio
```
## 📁 How to Use
Place your image files (e.g., image1.jpg, image2.jpg, image3.jpg, etc.) in the project directory.

Run the following Python script:


```
import imageio.v3 as iio

filenames = ['image1.jpg', 'image2.jpg', 'image3.jpg']
images = []

for filename in filenames:
    images.append(iio.imread(filename))

iio.imwrite('output.gif', images, duration=10, loop=0)
```
The script will generate an animated GIF named output.gif.

⚙️ Parameters
Parameter	Description	Example
duration	Time per frame in milliseconds	10
loop	Number of times the GIF should repeat	0 (infinite loop)

## 📌 Notes
Make sure all input images are the same dimensions for smooth playback.

You can adjust the duration to control the speed of the animation.
