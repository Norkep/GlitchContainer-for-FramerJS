# Glitch Container

A simple way to add glitch effect to your prototypes. Works with any layers.

This module using ```CSS filters```, ```Css blend modes```,  ```copy()``` method for layers and ```requestAnimationFrame```

![Screenshot one](/repo_img/preview-1.gif?raw=true "Screenshot one")
![Screenshot two](/repo_img/preview-2.gif?raw=true "Screenshot two")

A Fan overclocking alert! Don't overuse this container :-)

At this moment don't support dynamic textLayers, but you could reach all layers separately by name outside the class, like ```glitchA.layerRed.text = "example"```.

Also, you can create GlitchContainer from the group of layers.

```coffeescript
glitchA = new GlitchContainer
    layer: layerA #Your layer here
    speed: 40 #Speed of requestAnimationFrame updating
    stereoGlitch: true #Switch on red and blue filtered layers
    stereoOffsetX: 20 #Offset of red and blue filtered layers
    stereoOffsetY: 10
    blink: 0.6 #Correction coefficient for blinking 

glitchA.imgNoise() #Adding extra-layer "imgNoiseLayer" with base64 image

# Also, you could change some parametrs after GlitchContainer creation
glitchC.imgNoiseLayer.style.width = "200px" #Change any parameter, including noise-image

glitchA.speed = 20
glitchA.blink = 0.9
glitchA.stereoOffsetX = 50
glitchA.stereoOffsetY = 70
```

[Demo example](https://framer.cloud/KXWLF)


### Any questions or wishes

[open an issue](https://github.com/markdown-it/markdown-it) or [catch me on Facebook](https://www.facebook.com/pavel.laptev.94), also, you can [send me an e-mail](mailto:graphics.dario@gmail.com)