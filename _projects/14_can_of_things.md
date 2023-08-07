---
name: Can of Things
tools: [Computer Vision, C, Servos]
image: /assets/can-of-things/can.png
description: A trash can that can classify and sort waste - A 24hr hackathon project
---

# Can of Things

Two friends and I teamed up to build a smart trash can that can sort 6 different types of waste, winning 3rd place at Cornell Makeathon. Our goal was to utilize servos, cameras, and computers to sustainability reduce landfill waste and encourage recycling.

On the software side,
We researched datasets for recyclable image classification and decided to use a combination of TrashNet (from Github) and Waste Classification Data (from Kaggle). We used a pretrained VGG-16 deep convolutional neural network, with our own custom classification head. Our model achieved an accuracy of 85% overall. We did some fine tuning and biased predictions towards ‘trash’, achieving 95% accuracy on the trash category in the end. 

After we get the prediction result, we send the information through serial ports to the arduino board in order to control the servo.

For hardware, we use laser cutting and 3D printing to build a prototype trash can. We also experimented with both digital and continuous servos.


<p class="text-center">
<iframe width="560" height="315" src="https://www.youtube.com/embed/ulE_ubsVDzs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</p>