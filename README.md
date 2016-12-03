## Example

![example](http://i.imgur.com/DV5izE9.jpg)


```
python letterspics.py parrott.jpg -t ppaarroott
```
Here you see both the original and the edited close togheter. Made with [juxtapose-py](https://github.com/powahftw/juxtapose-py)


# letters-pics
Python script that given an image as input and some parameter it create a similar looking image composed of colored letter

### Prerequisites

This script make uses of the Python Imaging Library: PIL. You need to install it before running it

You also need to provide a .ttf font in the script directory. The default one is natasha.ttf but you can use different ones by launching the script with

```
python letterspics.py <inputpath> -f arial [additional arguments]
```

### Usage

You can use it by launching like

```
python letterspics.py <inputpath> [additional arguments]
```

You can have a look at the addictional parameter with 

```
python letterspics.py -h
```

```
-t Text to use | Default is HELLOWORLD
-d Dimension of the Typeface | Default is 15
-f Font to use | Default is natasha
-bow | Black/White option. Default is False. Quite buggy
```

### Other Exemple 


```
python letterspics.py cat.jpg -t theinternetismadeofcats -d 15
```

![example](http://i.imgur.com/Deqg3sT.jpg)



### Final notes

On small image, to achive better result the script double the dimension, otherwise the image's dimensions shouldn't change

The color frequency part of the script is based on [this](http://blog.zeevgilovitz.com/detecting-dominant-colours-in-python/).
It uses Colour Frequency since in a fraction of an image it's a good guess at what the average color is

The first Example image was created with another script which i created for the occasion[juxtapose-py](https://github.com/powahftw/juxtapose-py)

This script was developed in a short timeframe and as such there might be some occasional problem and some better optimization possibile. I appreciate any type of feedback :) 

