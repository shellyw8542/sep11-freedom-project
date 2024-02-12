# Entry 3
##### 02/12/2024

Through this blog, I would continue learning more about my tool, and find things that seem interesting for me in the A-frame website. I've been communicating a lot with my partner about the A-frame format, she would often give me some websites to visit and some tutorials. 

After a discussion with Shubata about the A-frame formatting, we decided that we would like to do something that seemed fun. I found something that we would both enjoy: [Animation](https://aframe.io/docs/1.5.0/components/animation.html) and [Laser-Controls](https://aframe.io/docs/1.5.0/components/laser-controls.html), we decided to pick one that is more interesting towards each other, and I picked laser control while Shubata did animation. For the struggle of Laser-Controls, it was hard to test the animation because the controls would normally use controllers and a VR set. However, there were some things that I took away from this lesson, I've learned the shortcut of DoF, which stands for Degree of Freedom. This means that it has movement in a limited space. The laser control requires a rotation, input, and laser-based interaction. The laser controls are a bunch of components, but by itself it does nothing. Some components are: [vive-controls](https://aframe.io/docs/1.5.0/components/vive-controls.html), [oculus-touch-controls](https://aframe.io/docs/1.5.0/components/oculus-touch-controls.html), and [windows-motion-controls](https://aframe.io/docs/1.5.0/components/windows-motion-controls.html). The vive-controls are for VR controls, it is used for controls from different uses to complete a game. For example, things like controllers, buttons, hands, models, etc. A format of this is: `<a-entity vive-controls="hand: left"></a-entity>` It also goes the same for Oculus touch controls and Windows motion controls. The difference is the formation and whatever the platform is suitable for. `<a-entity windows-motion-controls="hand: left"></a-entity>`. In the laser control, I would also need to know about the cursor and raycaster, which I learned before from past weeks ago. However, the point of having a cursor is to help visualize the area that the cursor is in, while the raycaster is used to draw the laser. 

Eventually, I found a [tutorial](https://www.youtube.com/watch?v=vQ85u3dzmZY) to help me fully understand the process and what I've learned. The tutorial recommends downloading Foxfire to help with a visual representation of the VR.
```
<a-scene school-playground>
    <a-entity superhands d="rightHand" hand-controls="hand: right: handModelStrle: lowPoly; color:black></a-entity>laser-controls="hand: left"></a-entity>
  <a-box
    position="-1.5 1.5 -3"
     color="yellow"
      animation="property:rotation; from: 0 0 0 to: 360 360 0; dur:2000; startEvents:click;"
    ></a-box>
</a-scene>
```
As explained in the video, lowPoly is used for the hand controls --> it makes the model of the hand. I also got curious about the component "Superhands", this component can make the object more interactive by making it have the ability of being hoverable, clickable, grabbable, stretchable, draggable, and droppable. I found laser controls very difficult to deal with, I couldn't tinker much with it because I didn't want to download Foxfire at that time, and I didn't want to fully commit to understanding all the VR sets. I found it not as helpful for my freedom project but I would discuss laser controls and what I've learned with my partner. My partner believed that the laser controls weren't something that was going to be added to the game, however, it was a good experience and showed the possibility of A-frame. My partner explained a lot of what I've learned before in Animation, like loop, light, position, play, autoplay, and some basic components. 

After browsing the A-frame website, I saw something that interested me which was [obj-model](https://aframe.io/docs/1.5.0/components/obj-model.html). The function of this component is to load an image using an.MTL file, the obj model has two properties. One for file: `<a-asset-item id="tree-mtl" src="/path/to/tree.mtl"></a-asset-item>`, and the other is for the URL: `<a-entity obj-model="obj: url(...);` Another idea is [Mixin](https://aframe.io/docs/1.5.0/core/mixins.html). Mixins are used for reusing a statement, I would like to compare it to a variable in Javascript. It is a lot like storing a variable however you can customize it with different things in HTML, it is normally placed in an id. 
```
    <a-mixin id="red" material="color: red"></a-mixin>
    <a-mixin id="blue" material="color: blue"></a-mixin>
    <a-mixin id="cube" geometry="primitive: box"></a-mixin>
    <a-entity mixin="red cube"></a-entity>
    <a-entity mixin="blue cube"></a-entity>
```
This would appear for a red cube and a blue cube. If the element is like this `<a-entity mixin="red blue cube">` then it would appear as blue because it is the latest color/property. I find both obj-model and mixins convenient for my project because I can have easy access instead of rewriting the elements and properties, as well as rewriting more towards my code. 

Lastly, I was curious about the [Asset Management System](https://aframe.io/docs/1.5.0/core/asset-management-system.html), so I decided to learn more about it. This system is for support and better performance in the coding. It can be used for "preloading assets", which helps create games and help them load. Asset Management Systems use these two compounds <a-assist>, and <a-scene> to pair with these elements: <a-asset-item>, <audio>, <img>, and <video>.

```
  <a-assets>
  <video id="pig" src="pig.mp4">
  <audio id="oink" src="oink.mp3"></audio>
 </a-assets>
```
This coding doesn't create any load-outs or errors because it doesn't cause any trouble since there's no time limit. However, once the audio or video is done playing, it will usually replay.  
Preloading is another thing that is included with the Asset Management System. Preloading helps prevent wait time, however, you can prevent it from happening by using autoplay (for audio) and preload="auto" (for video). In which it would look something like this:
```
<a-scene>
  <a-assets>
    <audio src="something.mp3" autoplay></audio>
    <video src="random.mp4" preload="auto"></video>
  </a-assets>
</a-scene>
```
You can also customize it to make it have a timeout before it loads: `<a-assets timeout="3000">` <-- This goes by milliseconds so in total it is 3 seconds.  
I believe that the Asset Management System is quite helpful to understand because it explains the concept of preloading and the preventions of it to help with the audio, videos, and images and make the gameplay smoother to work with.  

I am currently still on the second step, going towards the third step of the Engineering Design Process where I am still researching more about my tool, but I am taking into consideration the components that would come in handy for my freedom project. Where I am also digging more in-depth with the components that can help with my project and things that I've learned in the past to help with and apply to new concepts. The next step in the Engineering Design Process is to continue with my brainstorming and start planning the layout of my project. Some takeaways that I've learned from tinkering with my tool are "How to read" and "Problem decomposition", while also using "Collaboration". I've used the skill of "How to read" to help me read articles and documents to learn about the component and how to use it for certain situations. I also used the skill of "Problem decomposition" by breaking some new concepts into different days and also learning laser controls and animation. I asked my partner to help me, and then we both gathered and discussed what we'd discovered. Throughout many blogs, I've been using the helpful skill of "Collaboration" to help with what to do next, what to focus on, and ask some questions that involve a lot with my partner. 


[Previous](entry02.md) | [Next](entry04.md)

