# Entry 4
##### 03/18/2024

Throughout this blog, I will be continuing to learn with my tool, while also applying it to my freedom project.

This is the part of the freedom project where I would be communicating a lot with my partner about what to start with in our topic. How can we build our MVP, and who is doing what? My partner and I communicate with each other and we found that we can do certain tasks together. We outlined what we needed in our project before going beyond MVP. We understood that we had to have an `environment`, `animation`, and `functions`. We would most like to use this `.addEventListener(click)` to let the player shoot whenever they click or press a button. For the environment, there would be more things that would be added to make it look realistic, including models like trees, houses, cars, roads, and "people". To help keep things more organized we decided to break up the work according to time. We agreed on working on the setting first because then it gives out the baseline or the models and then when we are finished with the MVP we can add more details to it later. 

Doing the environment, first, I thought it would be a little difficult because you would need to change the whole background and add some textures. However, when starting to code, I thought that we would be using the component of `360 image` or `360 video` to make it look like it was more realistic on the background. However, my partner found this component in A-frame called the [environment component](https://github.com/supermedium/aframe-environment-component) and a [video](https://www.youtube.com/watch?v=K_1RdCVuu98) for it. We applied the starting code for the environment, and we selected the environment of default for now. After that, we worked on some of the models. 

I've struggled a lot with the positioning of the models. I created a big building with no windows using the `<a-box>` which was simpler because it was an unlimited amount of space. However, when creating the window it was harder because I had to position the `<a-box>` inside of the big building. 
```
<a-box position="-7 0 12" color="#8b0000" width="4" height="20" depth="4"></a-box> // <-- this is the initial (building)
<a-box position="-7 0 12" color="##000c8b" width="1" height="1" depth="4"></a-box> // <-- this is the initial (window)
```
I didn't change the positioning of the window because I thought the only problem was the width and height. This shows only the building because it was too small for the big building and it overlapped the window. So then I tried:
```
<a-box position="-3.5 0 6" color="#8b0000" width="1" height="1" depth="3"></a-box> // <-- this is the initial (first window)
<a-box position="-6.2 5 12.8" color="#8b0000" width="1" height="1" depth="3"></a-box> // <-- this is the initial (finial window)
```
This made the window off the building, and it made it hard for me to fix, I also didn't know what was wrong because I split the building position in half
[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
