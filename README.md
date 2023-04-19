<div style="border: 1px solid black; width: 300px; height: 150px;">
  <div style="background-color: pink; width: 100%; height: 100%; position: relative; transition: transform 0.5s;">
    <h2 style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); text-align: center;">Hover over the box to tilt it!</h2>
  </div>
</div>

<script>
  const tiltBox = document.querySelector('.tilt-box');
  tiltBox.addEventListener('mousemove', (e) => {
    const tiltX = (e.pageX - tiltBox.offsetLeft) / 20;
    const tiltY = (e.pageY - tiltBox.offsetTop) / -20;
    tiltBox.style.transform = `rotateX(${tiltY}deg) rotateY(${tiltX}deg)`;
  });
  tiltBox.addEventListener('mouseleave', () => {
    tiltBox.style.transform = `rotateX(0deg) rotateY(0deg)`;
  });
</script>
