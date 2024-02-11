# Entry 3
##### 02/12/2024

Through this blog, I would continue learning more about my tool, and find things that seem interesting for me in the A-frame website. I've been communicating a lot with my partner about the A-frame format, she would often give me some websites to visit and some tutorials. 

After a discussion with Shubata about the A-frame formatting, we decided that we would like to do something that seemed fun. I found something that we would both enjoy: [Animation](https://aframe.io/docs/1.5.0/components/animation.html) and [Laser-Controls](https://aframe.io/docs/1.5.0/components/laser-controls.html), we decided to pick one that is more interesting towards each other, and I picked laser control while Shubata did animation. For the struggle of Laser-Controls, it was hard to test the animation because the controls would normally use controllers and a VR set. However, there were some things that I took away from this lesson, I've learned the shortcut of DoF, which stands for Degree of Freedom. This means that it has movement in a limited space. The laser control requires a rotation, input, and laser-based interaction. The laser controls are a bunch of components, but by itself it does nothing. Some components are: [vive-controls](https://aframe.io/docs/1.5.0/components/vive-controls.html), [oculus-touch-controls](https://aframe.io/docs/1.5.0/components/oculus-touch-controls.html), and [windows-motion-controls](https://aframe.io/docs/1.5.0/components/windows-motion-controls.html). The vive-controls are for VR controls, it is used for controls from different uses to complete a game. For example, things like controllers, buttons, hands, models, etc. A format of this is: `<a-entity vive-controls="hand: left"></a-entity>` It also goes the same for Oculus touch controls and windows motion controls. The difference is the formation and whatever the platform is suitable for. `<a-entity windows-motion-controls="hand: left"></a-entity>`. In the laser control, I would also need to know about the cursor and raycaster, which I've learnt before from past weeks ago. However, the point of having a cursor is to help visualize the area that the cursor is in, while the raycaster is used to draw the laser. 

Eventually, I found to watch a [tutorial](https://www.youtube.com/watch?v=vQ85u3dzmZY) to help me fully understand the process and what I've learned. The tutorial recommends to download foxfire to help with a visual representation of the VR.
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
As explained in the video, lowPoly is used for the hand controls --> it makes the model of the hand. I also got curious of the component "Superhands", this component can make the object more interactive by making it have the ability of being hoverable, clickable, grabbable, stretchable, draggable, and droppable. I found laser controls very difficult to deal with, I found not as helpful towards my freedom project but I would discuss about laser controls and what I've learn with my partner. 



[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
