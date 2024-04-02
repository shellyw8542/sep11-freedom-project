# Tool Learning Log

Current tool: ***[A-frame](https://aframe.io/)***

Project: **Shooter Game**

---

10/28/2023:
* I went the the [Getting Started](https://jestjs.io/docs/getting-started) to find the setup and a [youtube tutorial](https://www.youtube.com/watch?v=FgnxcUQ5vho&ab_channel=WebDevSimplified) Of the setup in jest. (benefits of jests)
* I tried to use the code that was provided on the website, however, I didn't understand what npm or yarn meant
* Reading if you need to have Jest [installed](https://stackoverflow.com/questions/69559370/jest-without-npm-or-yarn) in order to test the coding out
* When trying out the coding on [https://jestjs.io/docs/getting-started] for yarn in [JS Bin](https://jsbin.com/nibezeyeho/edit?js,console) it kept giving me errors or `https://jsbin.com/nibezeyeho/edit?js,console` meaning that I would have to download it.
* As for now, I will watch videos about Jest to see if it would fit into my coding style.

10/29/2023:
* Got to download Jestjs on my ide sandbox.

11/5/2023:
* Gotten to create a platform for jest runs
* Getting started had a test that you will need to "run npm" with
* It kept showing me an error on the JSON
* Decide to look at the backup tool (Aframe)
* Getting started for A-frame was pretty simple and jsbin friendly.
* Aframe needs to have <script> before the <a-scene>

11/13/2023:
* Discussed with Shubata about what do to for the freedom project
* Plan on using the [360](https://aframe.io/examples/showcase/sky/)
* Shubata gave me a [video](https://www.youtube.com/watch?v=ZFTSLHd7xgY)
* Another link from the demo in [A-Frame](https://github.com/aframevr/aframe/blob/master/examples/test/video/index.html)
* Considering both the video and the link they both have `video id (and/or) src` <-- this is a lot like the HTML img id (which gives the img variable a name) and src is the link or file for the video)
* `<videosphere src>` <-- for the 360 videos and depending on the video's length and width has a rotation [00, 00, 00]
* Loops
* Autoplay loop can be true or false (true means keep playing) (false stop playing)
* Came across an error with Jsbin when tinkering with the demo with autoplay false.
* When testing loops (with A-frame) right-click and turn off the loop.
* Play and Pause can be used by javascript `play-pause`

11/20/2023:
* Experimented with [Responsive UI](https://aframe.io/examples/showcase/responsiveui/)
* By using the Inspect Scene
* Whenever you click on the element it focuses on that element
* Uses `<a-entity>` for a lot of these elements and projects
* Decided to look at the [entity](https://aframe.io/docs/1.5.0/core/entity.html) element
* entity itself does not do anything
* The functions of entities are to attach `geometry`, `material`, and `light`
* Example: `<a-entity geometry="primitive: box" material="color: red"
          light="type: point; intensity: 2.0">`
* Adding this to the example made the model more realistic
* You can also add components  to the `<a-entity>` like camera or sound
* Add .(that type of component)
* I believe that using the `<a-entity>` seems more like an id in HTML however you could adjust and also put javascript in it as well

11/27/2023
* Shubata gave me a helpful [video](https://www.youtube.com/watch?v=HrLsr-nzZGA)
* I created a tinker place in my ide sandbox
* In the video it explains the `<a-cursor>`
* Explains that `<a-cursor>` when the player selects the object, the object is selected in the coding
* Raycaster is a way to extend a line towards a place and check if it is near or on another object/entity
* Fuse is a timer
* Fusetimeout is the amount of time in the timer <-- this goes my milliseconds
`<a-cursor fuse="true" fusetimeout="8000"></a-cursor>`
* When doing raycaster be careful and choose what object should be selected to be a raycaster because it will generally pick everything the player chooses
* Raycaster seems to have a small circle in the middle of the screen
`<a-entity camera position="0 2 0" look-control wasd-controls>`
* When camera positioning is also critical because  it starts the user off with this position
* Controls of look can make you move your cursor along with your POV so whenever you left-click it changes the POV
* Controls of wasd the POV would move forward, backward, sideways if you press wasd
* With the controls you have to be organized with them. If the controls of wasd are spelled wrong then the whole coding doesn't work.
* In the sandbox, following the video I couldn't access my website so I had to switch to jsbin
* Whenever doing the coding do it in jsbin and paste the coding to the sandbox so next time referring to that topic go back on the sandbox and try to keep it organized.

12/04/2023
* I went back to the A-frame and sought something that might be helpful towards our game.
* [Shadow](https://aframe.io/docs/1.5.0/components/shadow.html)
* Shadows are used for a more realistic touch in the model
* You would need to have `<a-entity light="type:directional; castShadow:true;" position="1 1 1"></a-entity>`
* The castShadow has to be true
* As well as the compound of [light](https://aframe.io/docs/1.5.0/components/light.html#configuring-shadows)
* The coding depends on what you would like on the model
* For `intensity` this is used to light up the top of the model.
* It can be used like: <a-entity light= intensity: 1.5 </a-entity>
* Another idea is positioning
* I thought that positioning was just to position the models' angle
* It made me curious about what positioning for light does
* Position is supposed to be for the light source when you can adjust where you want the light source to be from
* The coding for positioning is just like the other model coding: `position="1 1 1"`
--> blog 1

12/18/2023 - 1/8/2024
* Discuss what to learn with Shubata
* We wanted to learn about the components given in A-frame
* We would both be learning [Animation](https://aframe.io/docs/1.5.0/components/animation.html) and [Laser-control](https://aframe.io/docs/1.5.0/components/laser-controls.html)
* We decided to split up the work and whatever is more interesting for us
* I picked Laser-control and Shubata picked Animation
* DoF --> degree of freedom = movement in a limited space
* They require rotation, input, and laser-based interaction
* Laser controls contain a lot of different components to create different visuals, but it doesn't work.
* The compounds for Laser-controls are [vive-controls](https://aframe.io/docs/1.5.0/components/vive-controls.html), [oculus-touch-controls](https://aframe.io/docs/1.5.0/components/oculus-touch-controls.html), and [windows-motion-controls](https://aframe.io/docs/1.5.0/components/windows-motion-controls.html)
* For the [vive-controls](https://aframe.io/docs/1.5.0/components/vive-controls.html) you will need to understand the tracked controls (which are used for VR controls) <-- I believe that it won't be too useful for me since I cannot test it.
* Vive-controls are used for controls from different uses to complete a game. For example, controllers, buttons, hand, model, etc.
* In case we are going to use this feature, this would be an example of the code: `<a-entity vive-controls="hand: left"></a-entity>`
* The same goes to the [oculus-touch-controls](https://aframe.io/docs/1.5.0/components/oculus-touch-controls.html)and [windows-motion-controls](https://aframe.io/docs/1.5.0/components/windows-motion-controls.html)
* Those components explain the coding for the controls and how to code them
* Nextly, I will be focusing on the laser-controls, which besides all the controls, it needs the component of cursor and raycaster.
* Based on the document it explains that the cursor is used to help the certain area that is in the cursor is in.
* The Raycaster is used for the drawing of the lasers.
* I followed a [tutorial](https://www.youtube.com/watch?v=vQ85u3dzmZY&ab_channel=clarecreate) to get a clear understanding and to tinker the coding with them.
* The tutorial recommends using foxfire to help with a visual representation about the VR
* So far I gotten in my coding:
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
* As explained in the video
* The lowPoly in the hand-controls makes the model of the hand
* [Superhands](https://github.com/c-frame/aframe-super-hands-component) can make the object more interactive by making it have the ability of being hoverable, clickable, grabbable, stretchable, draggable, and droppable
* When trying to tinker with this coding, I realized how hard it can be to test the VR version.
* All that showed up in the coding for Jsbin was the yellow box, however it was interactive towards the keyboard and mouse.

1/13/2024
* I was browsing the official documents for the A-frame model
* Found something that interests me
* [obj-model](https://aframe.io/docs/1.5.0/components/obj-model.html)
* This is used for loading in an image but by using an.MTL file
* It would look something like this: `<a-asset-item id="tree-obj" src="/path/to/tree.obj"></a-asset-item>`
* The obj model has two properties:
* obj and mtl
* obj is more common than mtl because it uses the generic file
* You could use obj + mtl for url or filing
* File: `<a-asset-item id="tree-mtl" src="/path/to/tree.mtl"></a-asset-item>`
* URL: `<a-entity obj-model="obj: url(...);`

1/21 - 1/29/2024
* Digging deeper into the [Asset Management System](https://aframe.io/docs/1.5.0/core/asset-management-system.html)
* This system is for support and better performance in the coding
* Used for "preloading assets"
* Usually if you using A-frame, this is normally used for creating games and helping them load
* Normally you would use `<a-assist>` and `<a-scene>` with these elements
* `<a-asset-item>, <audio>, <img>, and <video>`
* Doesn't create any load-outs or errors if they have a time limit
Example:
```
  <a-assets>
  <video id="pig" src="pig.mp4">
  <audio id="oink" src="oink.mp3"></audio>
 </a-assets>
```
* After the time goes out for the audio and video replaying (depending on the coding)
* Preloading can be used to avoiding wait time for things to load
* Preventions of preloading audio and videos are:
* `autoplay` <- audio
* `preload="auto"` <- video
```
<a-scene>
  <a-assets>
    <audio src="something.mp3" autoplay></audio>
    <video src="random.mp4" preload="auto"></video>
  </a-assets>
</a-scene>
```
* You could have a timeout before reaching a scene (load)
* `<a-assets timeout="3000">`
* Ideally you would want the timer to be 3 seconds
* It also goes by muliseconds
* I think that with this system it might be helpful to understand because since imgs and videos that are planned to be used in our game

2/2/2024
* [Mixin](https://aframe.io/docs/1.5.0/core/mixins.html)
* Mixin is used to reuse common sets of compounds
* It is usually placed in an id
* For example:
```
    <a-mixin id="red" material="color: red"></a-mixin>
    <a-mixin id="blue" material="color: blue"></a-mixin>
    <a-mixin id="cube" geometry="primitive: box"></a-mixin>
```
* Then after that is in the `<a-assets>`
```
  <a-entity mixin="red cube"></a-entity>
  <a-entity mixin="blue cube"></a-entity>
```
* This should appear with a red cube and a blue cube.
* Due to the mixin taking all the command names and entering the color and properties in the entity
* The mixin, if it is combined with the names then would create an entity that combines all the things that were provided (that you commanded)
* If the mixin had two of the same properties (same color, or shape) the last one would appear
* `<a-entity mixin="red blue cube">`
* This would be red, but blue would show up because it is the last of the color
* Mixin is used for convenience when coding the same properties, and also combining properties
* I would most likely use this for my freedom project

--> blog 2

3/2/2024
* After creating the MVP, me and my partner decided to start working on the setting
* My partner found this [video](https://www.youtube.com/watch?v=K_1RdCVuu98) that could be helpful for us to do
* Also this [environment component](https://github.com/supermedium/aframe-environment-component)
* This environment component helps us find the setting for the game (just the visuals of the floor/map)
* After that we wanted to pick what type of environment we could pick out and we chose for now to do the default of it
* Me and my partner decided to build a model of a building to be used for later developments
* I struggled a lot with the placement of the windows
* I tried to shrink the box by putting width and height by 1
* Example:
```html
<a-box position="-7 0 12" color="#8b0000" width="4" height="20" depth="4"></a-box> // <-- this is the initial (building)
<a-box position="-7 0 12" color="#8b0000" width="1" height="1" depth="4"></a-box> // <-- this is the initial (window)
```
* I believe that it does still look a bit rectangle but it is covered in the building
* I changed the positioning to half of everything:
```html
<a-box position="-3.5 0 6" color="#8b0000" width="1" height="1" depth="3"></a-box> // <-- this is the initial (first window)
<a-box position="-6.2 5 12.8" color="#8b0000" width="1" height="1" depth="3"></a-box> // <-- this is the initial (finial window)
```
* The first window was off the building, which was hard for me to fix, and I also didn't know what was wrong because I split the building position into half
* Then after a few tinkering moments I found that increasing "0" and "12" in position would've been better because it could move the window more up in the building
* The width was too far for the range, so I would put not too much apart from the box position but relatively close to the initial position.
* Then my partner helped me create details for the building by using an image on by using "scr" in the model of the box
  ```
  <a-box src="https://i.imgur.com/mYmmbrp.jpg"
  ```
  3/4/2024
  * After working on my setting, it was time for the next step in the MVP
  * I had to do the buildings and cars
  * I communicated with my partner and split up the work with me doing the building and my partner doing the cars
  * For my building I've decided to use an image to make it look realistic to the model
  * `<a-box src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/..." position="-7 0 12" color="#FFFFFF" width="4" height="20" depth="4"></a-box>`
  * This makes it so that the image would be in the model of the box
  * Then after that it was time to make the road because I had some extra time to make it
  * My partner suggests I use an `<a-plane>`
  * I didn't know what that element fully does until my partner told me what it does
  * The <a-plane> is meant for the ground
  * So what we did was `<a-plane position="20 0 20" rotation="-90 0 0" color="#000000" width ="10" height="0.5"></a-plane>`
  * This made the road at the bottom and it had a limited space
  * Then to make that road realistic, we wanted to put the yellow line in the road
  * `<a-box position="17 0 12" color="#C4A484" width="8" height="12" depth="8"></a-box>`
  * The yellow line may be a bit longer than the road, however for now since we didn't fully finish the setting and we might need adjustments  

   3/24/2024
* My partner and I wanted to adjust some of the settings for this week
* My partner created more buildings and I wanted to create a new design
* I decided to make a new car
* For the car you would need to have different shapes/models
* I wanted to have a box, sphere, and triangle
* At first, I thought that I would use the width, length, and height features however it didn't work in my favor
* The length feature didn't do much for the box:
`<a-box position="-1 3 -5"color="red" width="10" length="30" height="5"></a-box>`
* I wanted to make the box wider so I used "depth" like the building:
  <a-box position="-1 3 -5"color="red" width="10" depth="3" height="5"></a-box>
* After that I made the wheels by using the sphere shape
```
  <a-sphere position="-4 1 -5" radius="1.25" color="#000000"></a-sphere>
      <a-sphere position="2 1 -5" radius="1.25" color="#000000"></a-sphere>
```
* Creating the car wasn't bad, it was the size of the car that made it difficult.
* I also created a window for the car by using a smaller box to fix in the bigger box
  ` <a-box position="2 4 -5"color="blue" width="2" height="2" depth="3.5"></a-box> `
* To see the actual window you would need to make the depth a little higher because then it won't cause a bug or issue in that certain area of the car

03/31/2024
* Me and my partner wanted to try to make it so when you press a key, you shoot
* However, after looking at the shooting functions for multiple videos I couldn't understand the coding that was happening in javascript 
* We had a lot of videos to help guide us like:
          * https://supermedium.com/aframe-super-shooter-kit/examples/supercraft/
          * https://www.youtube.com/watch?v=q3bjSDTgUAg
          * https://www.youtube.com/watch?v=SeV7RmjxfTY
          * https://www.youtube.com/watch?v=t5Hou5QsRiE
* We reviewed it and came to realize that they had this "codechanger" website
* We tried some coding with the codechanger website like: 
`<a-cursor intersection-spawn="Event: click' mixin:voxel;"><a-cursor>`
* This didn't change anything in the code and it also didn't have a function for it
* This was supposed to be the coding to help make the player able to shoot
* Then we wanted to see if it works on the video, so we tested the starter code provided: https://replit.com/@codechangers/Targets-Starter
* The starter code wasn't working so we checked the official website for "code changers"
* The official website was shutted down and then we didn't know how to start
* We tried to use event listener: `.addEventListener("keypress", function);` but we didn't know how to start it
* After we finished our discussion I went to try out the coding without codechanger
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
* That didn't work but it made the loading faster, and I might need a little more understanding about the `a-cursor` and `events`. In a-frame to continue with the function of shoot/throw
<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
