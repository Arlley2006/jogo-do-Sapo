<!DOCTYPE html>
<html>
<head>
  <title>Frogger - Apenas Rua</title>
  <meta charset="UTF-8">
  <style>
    html, body {
      height: 100%;
      margin: 0;
    }

    body {
      background: black;
      display: flex;
      align-items: center;
      justify-content: center;
    }
  </style>
</head>
<body>
<canvas width="624" height="720" id="game"></canvas>
<script>
const canvas = document.getElementById('game');
const context = canvas.getContext('2d');

const grid = 48;
const frogger = { x: grid * 6, y: grid * 13, size: grid, color: 'greenyellow' };
const vehicles = [];

// Criando várias faixas de trânsito
const lanes = 10; // Aumentado para substituir o rio
for (let i = 1; i < lanes; i++) {
  let speed = (i % 2 === 0) ? 1.5 : -1;
  vehicles.push({ x: grid * (i % 5), y: grid * i, size: grid * 2, speed, color: '#c2c4da' });
}

function drawFrogger() {
  context.fillStyle = frogger.color;
  context.fillRect(frogger.x, frogger.y, frogger.size, frogger.size);
}

function drawVehicles() {
  vehicles.forEach(vehicle => {
    context.fillStyle = vehicle.color;
    context.fillRect(vehicle.x, vehicle.y, vehicle.size, grid);
    vehicle.x += vehicle.speed;
    if (vehicle.x > canvas.width) vehicle.x = -vehicle.size;
    if (vehicle.x + vehicle.size < 0) vehicle.x = canvas.width;
  });
}

function checkCollision() {
  return vehicles.some(vehicle => (
    frogger.x < vehicle.x + vehicle.size &&
    frogger.x + frogger.size > vehicle.x &&
    frogger.y < vehicle.y + grid &&
    frogger.y + frogger.size > vehicle.y
  ));
}

function loop() {
  requestAnimationFrame(loop);
  context.clearRect(0, 0, canvas.width, canvas.height);
  drawVehicles();
  drawFrogger();
  if (checkCollision()) {
    frogger.x = grid * 6;
    frogger.y = grid * 13;
  }
}

document.addEventListener('keydown', function(e) {
  if (e.key === 'ArrowLeft') frogger.x -= grid;
  if (e.key === 'ArrowRight') frogger.x += grid;
  if (e.key === 'ArrowUp') frogger.y -= grid;
  if (e.key === 'ArrowDown') frogger.y += grid;
  
  frogger.x = Math.max(0, Math.min(frogger.x, canvas.width - grid));
  frogger.y = Math.max(0, Math.min(frogger.y, canvas.height - grid));
});

loop();
</script>
</body>
</html>
