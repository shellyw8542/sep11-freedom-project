# Entry 2
##### 12/18/2023
When learning my tool in A-frame, there are a lot of new concepts in A-frame for HTML and Javascript. My partner and I would normally talk about what we plan to learn for the week and what we can use for our freedom project. My partner, Shubata, has more experience in A-frame than I do, so I needed to understand some of the context and basic HTML first to understand what to do next. I understood and watched a lot of tutorials about some different projects about A-frame. I've learned some important components to help with my shooter game.   

When following a [tutorial](https://www.youtube.com/watch?v=ZFTSLHd7xgY&ab_channel=DaniloPasquariello) for a 360 point of view, I felt that A-frame had a lot of custom and straightforward elements. For example, the video explains `video id` the purpose of this element is to help show the background of that component with a video. To this, I tried to create a video background but encountered a problem. When getting a video to put in my coding. Nothing would work. 
```
   <a-scene>
      <video id= "gif" scr ="(video link)" </video>
      </a-scene>
```
This is the coding that I applied towards Jsbin, however, it gave me a blank screen. After that, I tried a different video, I thought and believed that it was the video problem since I used a GIF. When I returned to the video I saw that the video had different components like `<a-assist>` and `<a-videosphere>`. I believed that since it was a lot like `<img>` perhaps it doesn't matter if I added nothing after. However, that wasn't the case when I modified the coding it turned into this:   
```
    <a-scene>
      <a-asset>
      <video id= "gif" scr ="(video link)" </video>
    <a-videosphere src="#gif" rotation="0 -90 0"></a-videosphere>
        </a-asset>
      </a-scene>
```
This coding helped me understand the concept of `<a-asset>` more, it is supposed to be a portion of coding to load. Another thing that I've learned was `<a-videosphere>`, while doing the video, I also learned about `loops`. Learning loops have an `autoplay` that can be true or false. True means it would continuously play and False would make it play once. 
This would be how the coding would look like:
```
<video id = "gif" autoplay loop="false" scr ="(video link)"</video>
```
When I played this on Jsbin, the autoplay remained as true, I tried to change the coding taking away the autoplay loop but it didn't work. I tried refreshing but it still didn't work, when I right-clicked the video, it showed a loop function and you can turn it off or on. There is another idea of play and pause, which can be expressed in Javascript as a function with `if and else` statements. I believe I probably will not use it but I got a peak about how the function works from the tutorial.  

[Responsive UI](https://aframe.io/examples/showcase/responsiveui/) seemed new to me and I wanted to see how it works. I tried tinkering with the A-frame example by using the `Inspect Scene`. After doing a bit of observation, I realized that there is a lot of `<a-entity>` in elements. I decided to check out the `entity` element in A-frame. I've learned that the element of `entity` itself doesn't do anything but rather it can have attachments like `geometry`, `material`, and `light`. For example:  
```
<a-entity geometry="primitive: box" material="color: red" light="type: point; intensity: 2.0">
```
This coding makes the model more realistic because the light becomes like a shadow and the intensity is the scaling of lightness. You can also link the entity to components like `.querySelector('aentity[camera]').components.camera`. In a sense, I observed that the element of `<a-entity>` was a lot like a regular id in HTML, however, the only difference was that you can adjust it. The connection is that you can link it with Javascript and like an id it contains a certain amount of elements.   

Another idea that the tool A-frame sparked my interest was the visuals and interaction that I wanted to learn. Now I finally have the opportunity to learn it. Shubata gave me this [video](https://www.youtube.com/watch?v=HrLsr-nzZGA&ab_channel=UWRealityLab) to help me understand more about the interactions in A-frame and how to code them. I believe that this is very helpful for my project because I wanted it to be interactive on the keyboard. In the video, it shows the element of `<a-cursor>` and  `wasd-controls`, the `wasd-controls` can make the camera move. For example `w` would move forward, `a` would move to the left, and so on. `<a-cursor` is for mouse controls. But what does this look like in coding?  
```
   <a-scene>
        <a-entity camera position="0 2 0" look-control wasd-controls>
          <a-cursor id="cursor" fuse="true" fusetimeout="3000"></a-cursor>
        </a-entity>
      </a-entity>
   </a-scene>
```
Something that I was curious about in the coding was the camera positioning. What was the point of having the positions if you can control the model's point of view? I tried to add different numbers for the length and height and it turns out that the positioning is only for the camera's initial position. I've also learned more about fuse, which might also be helpful for my project. Fuse's function is basically like a timer and a `fusetimeout` gives the number of that timer in seconds. So it'll be `<a-cursor fuse="true" fusetimeout="8000"></a-cursor>`. While watching the tutorial I came across the component of `Raycaster`. A raycaster is a way to extend a line towards a place and check if it is near or on another object/entity. When I was coding the Raycaster, I saw that in the middle of the screen, it showed a circle as described in the coding above.  

Lastly, I wanted to learn and explore components that can help with my project. I found [shadows](https://aframe.io/docs/1.5.0/components/shadow.html) in the A-frame documents and learned that shadows are used to have a realistic style. How does it look like though?  
```
<a-entity light="type:directional; castShadow:true;" position="1 1 1"></a-entity>
```  
The castShadow as to be true to have the shadow in the model. But shadows link to the function of [light](https://aframe.io/docs/1.5.0/components/light.html#configuring-shadows). Within that, you can also use `intensity` for a certain type of light tone as explained before. While learning about `light` I had a question that came up in mind, Why does light need to have positioning? I tinkered from the example given and changed the positioning into `position="1 1 1"` thus changing the position of the light that it is coming from. 

I am currently in the second step of the Engineering Design Process where I am researching to learn more about my tool and gather information and components to help my freedom project. The next step of the Engineering Design Process is to continue with my research as well as start designing and digging into deeper information about some topics for my project. Some takeaways that I've learned while tinkering with my tools were: Consideration, How to learn, and Communication. When I started to be optimistic about my tool, I learned a lot of new and important things that can be helpful with my freedom project. I learned by trying things out on Jsbin, watching tutorials about those components, asking questions, and reading from the website. I've been taking into consideration the components that might help in my project. Lastly, I've been communicating throughout the weeks with my partner to help her decide on what to do and what should we do next. I also ask my partner for help in case I do not understand the problem with my coding. 
