# Indian-Dishes-Classifier
The only Classifier you need to Classify your Indian Dishes. <a href='https://ai-maharaj.herokuapp.com/'> Try It! </a> <br>
<a href='https://github.com/deeprodge/Indian-Dishes-Classifier'> Deployement code here.</a>

## What it does
It is an Image Classifier that can classifiy images into 12 different Indian Dishes, which includes Chole Bhature, Pav Bhaji, Paneer Sabzi, Momos, Biryani, Butter Naan, Dhokla, Samosa, Chai, Jalebi, Gulab Jamun, Rasgulla.

## Challenges I ran into

- Couldn't find a Indian Dishes Dataset, So had to create the dataset manually
- Couldn't find a Google Image Scraper, So I made a custom Google Image scraper script which can scrape multiple classes of images at a single time.
- The Dataset had only around 4000 images, So I used Data Augmentation to Augment Data.
- The training cost was not decreasing even in the initial stage, So I had to start from a different random point with larger learning rate.
- First I used ResNet101 model for transfer learning, but the model was too heavy to be run on heroku, So I changed the model and used EfficientNet-b2 as it a mobile model.

## What I learned

- Transfer Learning Using PyTorch
- Deployment of model using Flask and Heroku
- Using LR Scheduler to decrease Learning Rate with epochs

```
MIT License

Copyright (c) 2021 Deep Rodge

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

