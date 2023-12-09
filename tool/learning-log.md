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
* Play and Pause can be used by javascript `play-pause` in HTML

11/20/2023:
* Experimented with [Responsive UI](https://aframe.io/examples/showcase/responsiveui/)
* By using the Inspect Scene 
* Whenever you click on the element it focuses on that element
* Uses `<a-entity>` for a lot of these elements and projects
* Decided to look at the [entity](https://aframe.io/docs/1.5.0/core/entity.html) element
* entity's itself does not do anything
* The functions of entity's is to attach `geometry`, `material`, and `light`
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
* With the controls you have to be organized with it. If the controls of wasd are spelled wrong then the whole coding doesn't work.
* In the sandbox, following the video I couldn't access my website so I had to switch to jsbin
* Whenever doing the coding do it in jsbin and paste the coding to the sandbox so next time referring to that topic go back on the sandbox and try to keep it organized. 

12/04/2023
* I went back to the A-frame and seeked something that might be helpful towards our game.
* [Shadow](https://aframe.io/docs/1.5.0/components/shadow.html)
* Shadows are used for a more realistic touch in the model
* You would need to have `<a-entity light="type:directional; castShadow:true;" position="1 1 1"></a-entity>`
* The castShadow has to be true
* As well as the compound of `[light](https://aframe.io/docs/1.5.0/components/light.html#configuring-shadows)`
* The coding depends on what you would like on the model
* For `intensity` this is used to light up the top of the model.
* It can be used like: <a-entity light= intensity: 1.5 </a-entity>
* I didn't understand what the position meant
* Position is supposed to be for the light source when you can adjust where you want the light source to be from 





<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
