# Entry 5
##### 05/06/24
During the multiple days of doing the freedom project, and communicating with my partner about how to work with our project within a matter of weeks with the tool that we've learned. 

When creating our outline for our MVP, we decided to break up the task to do and what to do. After working on the environment component and some buildings, we wanted to work on our shooting ability. Initially, we thought that the shooting ability could be used with the website that was being provided by a few videos like the [Target shooting game](https://www.youtube.com/watch?v=q3bjSDTgUAg), [Building a shooting game](https://www.youtube.com/watch?v=SeV7RmjxfTY), and the example of [Supercraft Shooter](https://supermedium.com/aframe-super-shooter-kit/examples/supercraft/). We had everything planned for this game, however it wasn't working how we wanted it to work. We tried to find the source that provided the javascript functions, which was called "codechangers". At first in the videos, I went to the link that was provided and saw that they used `<a-cursor intersection-spawn="Event: click' mixin:voxel;"><a-cursor>`. When trying out this code, the code wasn't working out. The function in the video made it so that when you click on the cursor, the cursor would do something, in which I wanted to create a ball if clicked. I double-checked another [link](https://replit.com/@codechangers/Targets-Starter) that had "codechangers" however, the starter code didn't work either. Me and my partner tried to look at the official website but we couldn't get in because it had been closed. My partner believed that the website would open again because the website worked before we started coding. 

I suggested many ideas like using an event listener or combining a new tool. For the `.addEventListener("keypress", function); ` I didn't know how to really start with my coding and found that it wouldn't really work. I tried using the code without codechangers:
```
    <script src="https://cdnjs.cloudflare.com/ajax/libs/aframe/1.5.0/aframe.min.js"></script>
    <script src="https://unpkg.com/aframe-environment-component@1.1.0/dist/aframe-environment-component.min.js"></script>  
  </head>
  <body>
    <a-scene id="myScene">
      <a-entity environment="preset:forest;"></a-entity>
      <a-plane id="floor" static-body height="1000" width="1000" position="0 -0.02 0" color="black" rotation="-90 0 0"></a-plane>
      <a-camera id="myCamera" position="0 1 0">
        <a-cursor = "event: keypress; mixin: voxel"></a-cursor>
```
It didn't work out because it was specialized only using codechangers, I thought that the codechangers and a-frame would be somewhat alike. I remembered that there was a tool that was like a-frame but more js related. It was called [three.js](https://threejs.org/). I found that using three.js was quite helpful, in three.js there was a [physics](https://threejs-journey.com/lessons/physics#ammo-js) component as well as a [guidance video](https://www.youtube.com/watch?v=30bO8SBIZYw). Throughout the video, I realized that you would need to use a raycaster when shooting a ball.
```
function onMouseDown(event){
          mouseCoords.set // set the mouse on the origin
          (event.clientX / innerWidth) * 2 - 1,
          - (event.clientY / innerHeight) * 2 + 1
);
raycaster.setFromCamera(mouseCoords,Camera)
```
This coding would help you set the camera towards the middle of the screen and then you would need to use this raycaster function to make your mouse do something after it shoots. 
```
function addEventHandlers(){
          event.addEventListener('mousedown', onMouseDown, false)
```
I introduced my idea of the usage of three.js and how it could help with our functions with shooting. The physics function would help make the ball that is being shot slowly go down over time. My partner agreed with the idea and I installed three.js and tried to combine it with the project. The coding is in three.js was very confusing because I didn't understand what is the coding for most of the components. I found the concept of raycasters on three.js and found that it can be used for many purposes like showing the distance between the cameras directly from the raycaster's position. 
```
renderer.domElement.addEventListener('mousemove', onMouseMove, false)

function onMouseMove(event: MouseEvent) {
    const mouse = {
        x: (event.clientX / renderer.domElement.clientWidth) * 2 - 1,
        y: -(event.clientY / renderer.domElement.clientHeight) * 2 + 1
    } as THREE.Vector2

         console.log(mouse)

         raycaster.setFromCamera(mouse, camera);
```
This code makes it so that when the mouse is being moved it is also being recorded by the raycaster. So that the next movement can be interactive from based on the previous movement. 


[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
