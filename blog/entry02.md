# Entry 2
##### 12/18/2023
When learning my tool in A-frame, there are a lot of new concepts in A-frame for HTML and Javascript. My partner and I would normally talk with each other about what we plan to learn for the week and what we can use for our freedom project. My partner, Shubata, has more experience in A-frame than I do, so I needed to understand some of the context and basic HTML first to understand what to do next. I understood and watched a lot of tutorials about some different projects about A-frame. I've learned some important components to help with my shooter game.   
When following a [tutorial](https://www.youtube.com/watch?v=ZFTSLHd7xgY&ab_channel=DaniloPasquariello), I felt that A-frame had a lot of custom and straightforward elements. For example, the video explains `video id` the purpose of this element is suppose to help show the background of that component with a video. To this, I tried to create a video background however, I came across a problem. When getting a video to put in my coding. Nothing would work. 
```
   <a-scene>
      <video id= "gif" scr ="(video link)" </video>
      </a-scene>
```
This is the coding that I applied towards Jsbin, however, it gave me a blank screen. After that, I tried a different video, I thought and believed that it was the video problem since I used a GIF. When I went back to the video I saw that the video had different components like `<a-assist>` and `<a-videosphere>`. I believed that since it was a lot like `<img>` perhaps it doesn't matter if I added nothing after. However that wasn't the case when I modified the coding it turned into this:   
```
    <a-scene>
      <a-asset>
      <video id= "gif" scr ="(video link)" </video>
    <a-videosphere src="#gif" rotation="0 -90 0"></a-videosphere>
        </a-asset>
      </a-scene>
```
This coding helped me understand the concept of `<a-asset>` more, it is supposed to be a portion of coding to load. Another thing that I've learned was `<a-videosphere>`, this element's function is to adjust the `geometry` and `rotation` of the video by using the `<video id>`.  
Another idea that the tool A-frame sparked my interest was the visuals and interaction that I wanted to learn. Now I finally have the opportunity to learn it. Shubata gave me this [video](https://www.youtube.com/watch?v=HrLsr-nzZGA&ab_channel=UWRealityLab) to help me understand the interactions and how to code them. 


[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)
