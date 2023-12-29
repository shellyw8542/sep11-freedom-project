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
When I played this on Jsbin, the autoplay remained as true, I tried to change the coding taking away the autoplay loop but it didn't work. I tried refreshing but it still didn't work, when I right-clicked the video, it showed a loop function and you can turn it off or on. You can also use the play and pause functions described in Javascript.
Another idea that the tool A-frame sparked my interest was the visuals and interaction that I wanted to learn. Now I finally have the opportunity to learn it. Shubata gave me this [video](https://www.youtube.com/watch?v=HrLsr-nzZGA&ab_channel=UWRealityLab) to help me understand more about the interactions in A-frame and how to code them. I believe that this is very helpful for my project because I wanted it to be interactive on the keyboard. In the video, it shows the element of `<a-cursor>` and  `wasd-controls`, the `wasd-controls` can make the camera move. For example `w` would move forward, `a` would move to the left, and so on. `<a-cursor` is for mouse controls. But what does this look like in coding?  
```
   <a-scene>
        <a-entity camera position="0 2 0" look-control wasd-controls>
          <a-cursor id="cursor" fuse="true" fusetimeout="3000"></a-cursor>
        </a-entity>
      </a-entity>
   </a-scene>
```
Something that I was curious about in the coding was the camera positioning. What was the point of having the positions if you can control the model's point of view? I tried to add different numbers for the length and height and it turns out that the positioning is only for the camera's initial position. I've also learned more about fuse, which might also be helpful for my project. Fuse's function is basically like a timer and a `fusetimeout` gives the number of that timer in seconds. So it'll be `<a-cursor fuse="true" fusetimeout="8000"></a-cursor>`.  

I am currently in the second step of the engineering design process where I am researching to learn more about my tool and gather information and components to help my freedom project. Some takeaways that I've learned while tinkering with my tools were: Consideration, How to learn, and Communication. When I started to be optimistic about my tool, I learned a lot of new and important things that can be helpful with my freedom project. I learned by trying things out on Jsbin, watching tutorials about those components, asking questions, and reading from the website. I've been taking into consideration the components that might help in my project. Lastly, I've been communicating throughout the weeks with my partner to help her decide on what to do and what should we do next. I also ask my partner for help in case I do not understand the problem with my coding. 
