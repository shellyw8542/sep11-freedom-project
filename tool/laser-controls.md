<html>
  <head>
    <script src="https://aframe.io/releases/1.5.0/aframe.min.js"></script>
  <script src="https://cdn.jsdelivr.net/gh/donmccurdy/aframe-extras@v6.1.1/dist/aframe-extras.misc.min.js"></script>
  <script src="https://unpkg.com/super-hands@^3.0.3/dist/super-hands.min.js"></script>
  </head>
  <body>
<a-scene school-playground>
    <a-entity superhands d="rightHand" hand-controls="hand: right: handModelStrle: lowPoly; color:black></a-entity>laser-controls="hand: left"></a-entity>
  <a-box
    position="-1.5 1.5 -3"
     color="yellow"
      animation="property:rotation; from: 0 0 0 to: 360 360 0; dur:2000; startEvents:click;"
    ></a-box>
</a-scene>
  </body>
</html>