---
title: "Orientation network"
excerpt: "Detect an oriented bounding box aligned with an animal's body.<br/><img src='/images/portfolio_wbia_orientation.jpg'>"
collection: portfolio
---

The aim of the project is to detect object-aligned bounding box based on axis-aligned bounding box. 
Axis-aligned bounding box is a common output of object detection methods.
Due to large variations in poses of animals in images especially for underwater images, axis-aligned box is not sufficient for furhter analysis of the detected animal, e.g. identification/matching of specific individual.
Detecting orientation and object-aligned box allows to normalize poses of the animals to a commont view by croping and rotating images.
The project trains a convolutional neural network to learn oriented rectangles that provide the direction of the animal.

The project is completed for [WildMe/WildBook](https://www.wildme.org) based on their data.
The source code, implementation details and results are available at [github](https://github.com/WildMeOrg/wbia-plugin-orientation).

The method is generic and not species specific. The same model architecture and training schedule are applied to seven species including turtles, manta rays, whale sharks, right whales and sea horses.


Examples of detected orientation.
Green box - axis-aligned detection rectangle provided as input.
Read box with yellow dashed line - detected oriented object-aligned rectangle.

![Example of spotted dolphing](/images/portfolio-wbia-orientation-dolphins.jpg)

![Example of oriented turtles](/images/portfolio-wbia-orientation-turtles.jpg)

![Example of manta rays](/images/portfolio-wbia-orientation-mantas.jpg)

![Example of right whales](/images/portfolio-wbia-orientation-right-whales.jpg)


Image credit: [WildMe/WildBook](https://www.wildme.org)
