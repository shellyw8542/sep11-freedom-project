# Entry 4
##### 03/18/2024

Throughout this blog, I will be continuing to learn with my tool, while also applying it to my freedom project.

This is the part of the freedom project where I would be communicating a lot with my partner about what to start with in our topic. How can we build our MVP, and who is doing what? My partner and I communicate with each other and we found that we can do certain tasks together. We outlined what we needed in our project before going beyond MVP. We understood that we had to have an `environment`, `animation`, and `functions`. We would most like to use this `.addEventListener(click)` to let the player shoot whenever they click or press a button. For the environment, there would be more things that would be added to make it look realistic, including models like trees, houses, cars, roads, and "people". To help keep things more organized we decided to break up the work according to time. We agreed on working on the setting first because then it gives out the baseline or the models and then when we are finished with the MVP we can add more details to it later. 

Doing the environment, first, I thought it would be a little difficult because you would need to change the whole background and add some textures. However, when starting to code, I thought that we would be using the component of `360 image` or `360 video` to make it look like it was more realistic on the background. However, my partner found this component in A-frame called the [environment component](https://github.com/supermedium/aframe-environment-component) and a [video](https://www.youtube.com/watch?v=K_1RdCVuu98) for it. We applied the starting code for the environment, and we selected the environment of default for now. After that, we worked on some of the models. 

I've struggled a lot with the positioning of the models. I created a big building with no windows using the `<a-box>` which was simpler because it was an unlimited amount of space. However, when creating the window it was harder because I had to position the `<a-box>` inside of the big building. 
```
<a-box position="-7 0 12" color="#8b0000" width="4" height="20" depth="4"></a-box> // <-- this is the initial (building)
<a-box position="-7 0 12" color="#87CEEB" width="1" height="1" depth="4"></a-box> // <-- this is the initial (window)
```
I didn't change the positioning of the window because I thought the only problem was the width and height. This shows only the building because it was too small for the big building and it overlapped the window. So then I tried:
```
<a-box position="-3.5 0 6" color="#87CEEB" width="1" height="1" depth="3"></a-box> // <-- this is the initial (first window)
<a-box position="-6.2 5 12.8" color="#87CEEB" width="1" height="1" depth="3"></a-box> // <-- this is the initial (finial window)
```
This made the window off the building, and it made it hard for me to fix, I also didn't know what was wrong because I split the building position in half of the original building. After many attempts to find a good position for a window, I found that you need to change the x and y axis. You need to keep the positioning relatively close to the initial position of the big building. So the final coding of the model should be:
```
            <a-scene>
              <a-entity environment="preset: default; dressingAmount: 500"></a-entity>
                <a-box position="-7 0 12" color="#8b0000" width="4" height="20" depth="4"></a-box>
                <a-box position="-6.2 5 12.8" color="#87CEEB" width="1" height="1" depth="3"></a-box>
                <a-box position="-6.2 3 12.8" color="#87CEEB" width="1" height="1" depth="3"></a-box>
                 <a-box position="17 0 12" color="#C4A484" width="8" height="12" depth="8"></a-box>
      </a-scene>
```

After doing that model, my partner wanted to do the road, more buildings, and cars. I continuously did the buildings and my partner did the car's model. I wanted to make my building look more realistic so I used an image to help with the details.  
`<a-box src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/..." position="-7 0 12" color="#FFFFFF" width="4" height="20" depth="4"></a-box>`  
Adding the `src` made only the box have the image that I selected in the model. After finishing the model, I had time to create the road. My partner suggested I use the component of `<a-plane>` which is a platform at the bottom of the model you made. We added the road with limited space: `<a-plane position="20 0 20" rotation="-90 0 0" color="#000000" width ="10" height="0.5"></a-plane>` and to make it look more realistic we added `<a-box position="17 0 12" color="#C4A484" width="8" height="12" depth="8"></a-box>` for the yellow line. Although it isn't fully as we imagined, this model overall is good for us to continue. 

I am currently stages 4 and 5 in the Engineering Design Process where I planned out the MVP and now creating the prototype of my freedom project. The next step in the Engineering Design Process is to continue creating my project, reaching the MVP, and then testing my prototype. Some takeaways that I've gotten from this blog were: Problem decomposition and Time management. I believe that I've used problem decomposition to break down the freedom project into different parts in terms of weeks. I also used Time management to set a time when is a good time to work on the setting, animations, and functions. Also, I've been communicating with my partner about when is a good time to help do the project together.  

[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
