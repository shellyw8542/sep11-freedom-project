<html>
  <head>
  <script src="https://aframe.io/releases/1.5.0/aframe.min.js"></script>
  <script src="https://unpkg.com/aframe-environment-component/dist/aframe-environment-component.min.js"></script>
</head>
  <body>
    <a-scene>
<a-box position="-1 0.5 -3" rotation="0 45 0" color="#4CC3D9" animation="property: object3D.position.y; to: 2.2; dir: alternate; dur: 2000; loop: true"></a-box>></a-box>
      <a-sphere position="0 1.25 -5" radius="1.25" color="#EF2D5E"></a-sphere>
       <a-sphere position=".5 1.80 -4" radius=".2" color="#000000"></a-sphere>
      <a-sphere position="-.5 1.80 -4" radius=".2" color="#000000"></a-sphere>


      <a-cylinder src="https://i.imgur.com/mYmmbrp.jpg" position="1 0.75 -3" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
      <a-sky color="#ECECEC"></a-sky>
      <a-scene>
  <a-box color="red" position="0 2 -5" rotation="0 45 " scale="2 2 2"></a-box>


        <a-entity environment="preset: default; dressingAmount: 500"></a-entity>

</a-scene>
    </a-scene>
  </body>
</html>
