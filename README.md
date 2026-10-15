# kehidupan-abad-pertengahan
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>VR Kehidupan Abad Pertengahan</title>
  <script src="https://aframe.io/releases/1.7.1/aframe.min.js"></script>
</head>

<body>
<a-scene
  background="color: #B9D9E8"
  renderer="colorManagement: true"
  shadow="type: pcfsoft">

  <!-- Pencahayaan -->
  <a-light type="ambient" color="#FFFFFF" intensity="0.8"></a-light>
  <a-light type="directional" position="-4 8 5"
            intensity="1.5" cast-shadow="true"></a-light>

  <!-- Tanah dan jalan desa -->
  <a-plane rotation="-90 0 0" width="100" height="100"
           color="#78945A" shadow="receive: true"></a-plane>

  <a-plane rotation="-90 0 0" position="0 0.02 0"
           width="5" height="50" color="#BDA37A"></a-plane>

  <!-- Rumah penduduk -->
  <a-entity position="-5 0 -5">
    <a-box position="0 1 0" width="3" height="2"
           depth="3" color="#C69B72"></a-box>
    <a-cone position="0 2.5 0" radius-bottom="2.4"
            radius-top="0" height="1.5"
            color="#79513B"></a-cone>
    <a-box position="0 0.8 1.51" width="0.7"
           height="1.5" depth="0.08" color="#593B2B"></a-box>
    <a-box position="-0.9 1.3 1.54" width="0.45"
           height="0.45" depth="0.08" color="#83B7CC"></a-box>
  </a-entity>

  <!-- Rumah kedua -->
  <a-entity position="5 0 -7">
    <a-box position="0 1 0" width="3" height="2"
           depth="3" color="#D5B18A"></a-box>
    <a-cone position="0 2.5 0" radius-bottom="2.4"
            radius-top="0" height="1.5"
            color="#6D4938"></a-cone>
    <a-box position="0 0.8 1.51" width="0.7"
           height="1.5" depth="0.08" color="#593B2B"></a-box>
  </a-entity>

  <!-- Gereja desa -->
  <a-entity position="0 0 -13">
    <a-box position="0 2 0" width="4"
           height="4" depth="4" color="#D9D0BB"></a-box>
    <a-cone position="0 4.8 0" radius-bottom="3"
            radius-top="0" height="2"
            color="#51473F"></a-cone>
    <a-box position="0 4.4 0" width="0.18"
           height="1.2" depth="0.18" color="#E9D9A8"></a-box>
    <a-box position="0 4.6 0" width="0.7"
           height="0.15" depth="0.18" color="#E9D9A8"></a-box>
    <a-box position="0 1.3 2.02" width="1"
           height="2" depth="0.1" color="#684733"></a-box>
  </a-entity>

  <!-- Lapak pasar -->
  <a-entity position="-3 0 3">
    <a-box position="0 1 0" width="3"
           height="0.2" depth="1.5" color="#805638"></a-box>
    <a-box position="0 1.8 0" width="3.5"
           height="0.15" depth="2" color="#9E3930"></a-box>
    <a-cylinder position="-1.4 1.35 0.6"
                radius="0.06" height="1.2" color="#684733"></a-cylinder>
    <a-cylinder position="1.4 1.35 0.6"
                radius="0.06" height="1.2" color="#684733"></a-cylinder>
    <!-- Hasil bumi -->
    <a-sphere position="-0.7 1.3 0" radius="0.18" color="#CDA83D"></a-sphere>
    <a-sphere position="0 1.3 0" radius="0.18" color="#A74432"></a-sphere>
    <a-sphere position="0.7 1.3 0" radius="0.18" color="#71934D"></a-sphere>
  </a-entity>

  <!-- Lahan pertanian -->
  <a-entity position="7 0 3">
    <a-box position="0 0.08 0" width="7"
           height="0.15" depth="8" color="#765638"></a-box>
    <a-box position="0 0.17 -2" width="6.5"
           height="0.12" depth="0.12" color="#A17B4F"></a-box>
    <a-box position="0 0.17 0" width="6.5"
           height="0.12" depth="0.12" color="#A17B4F"></a-box>
    <a-box position="0 0.17 2" width="6.5"
           height="0.12" depth="0.12" color="#A17B4F"></a-box>

    <!-- Tanaman -->
    <a-cylinder position="-2 0.5 -2" radius="0.12"
                height="0.7" color="#668746"></a-cylinder>
    <a-cylinder position="0 0.5 -2" radius="0.12"
                height="0.7" color="#668746"></a-cylinder>
    <a-cylinder position="2 0.5 -2" radius="0.12"
                height="0.7" color="#668746"></a-cylinder>
    <a-cylinder position="-2 0.5 0" radius="0.12"
                height="0.7" color="#668746"></a-cylinder>
    <a-cylinder position="0 0.5 0" radius="0.12"
                height="0.7" color="#668746"></a-cylinder>
    <a-cylinder position="2 0.5 0" radius="0.12"
                height="0.7" color="#668746"></a-cylinder>
  </a-entity>

  <!-- Figur penduduk sederhana -->
  <a-entity position="-1 0 5">
    <a-cylinder position="0 1 0" radius="0.28"
                height="1.1" color="#526F9B"></a-cylinder>
    <a-sphere position="0 1.8 0" radius="0.25"
              color="#D9AC83"></a-sphere>
    <a-cone position="0 2.1 0" radius-bottom="0.35"
            radius-top="0.05" height="0.5" color="#604832"></a-cone>
  </a-entity>

  <a-entity position="2 0 4">
    <a-cylinder position="0 1 0" radius="0.28"
                height="1.1" color="#8B473D"></a-cylinder>
    <a-sphere position="0 1.8 0" radius="0.25"
              color="#C99470"></a-sphere>
    <a-cone position="0 2.1 0" radius-bottom="0.35"
            radius-top="0.05" height="0.5" color="#51402F"></a-cone>
  </a-entity>

  <!-- Judul dan keterangan -->
  <a-text value="KEHIDUPAN SOSIAL ABAD PERTENGAHAN"
          position="0 5 -4" align="center"
          width="12" color="#33271D"></a-text>

  <a-text value="Pasar: pusat perdagangan dan interaksi"
          position="-3 3 3" align="center"
          width="5" color="#33271D"></a-text>

  <a-text value="Gereja: pusat kehidupan keagamaan"
          position="0 5 -9" align="center"
          width="6" color="#33271D"></a-text>

  <a-text value="Pertanian: mata pencaharian utama"
          position="7 2 3" align="center"
          width="5" color="#33271D"></a-text>

  <!-- Kamera dan kontrol -->
  <a-entity position="0 1.6 12">
    <a-camera wasd-controls look-controls>
      <a-cursor color="#FFFFFF"
                raycaster="objects: .clickable"></a-cursor>
    </a-camera>
  </a-entity>

</a-scene>
</body>
</html>
