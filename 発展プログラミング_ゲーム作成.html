<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8" />
<title>よけゲーム（JavaScript版）</title>
<style>
  canvas {
    background: #eee;
    display: block;
    margin: 20px auto;
    border: 1px solid #333;
  }
</style>
</head>
<body>

<canvas id="gameCanvas" width="480" height="640"></canvas>

<script>
const canvas = document.getElementById('gameCanvas');
const ctx = canvas.getContext('2d');

const WIDTH = canvas.width;
const HEIGHT = canvas.height;

const playerSize = 50;
let playerX = WIDTH / 2 - playerSize / 2;
const playerY = HEIGHT - playerSize - 10;
const playerSpeed = 7;

const obstacleSize = 50;
let obstacleX = Math.random() * (WIDTH - obstacleSize);
let obstacleY = -obstacleSize;
let obstacleSpeed = 5;

let score = 0;
let gameOver = false;

let keys = {};

window.addEventListener('keydown', e => {
  keys[e.key] = true;
});

window.addEventListener('keyup', e => {
  keys[e.key] = false;
});

function update() {
  if (gameOver) return;

  // プレイヤー移動
  if (keys['ArrowLeft'] && playerX > 0) {
    playerX -= playerSpeed;
  }
  if (keys['ArrowRight'] && playerX < WIDTH - playerSize) {
    playerX += playerSpeed;
  }

  // 障害物移動
  obstacleY += obstacleSpeed;
  if (obstacleY > HEIGHT) {
    obstacleY = -obstacleSize;
    obstacleX = Math.random() * (WIDTH - obstacleSize);
    score++;
    if (score % 5 === 0) {
      obstacleSpeed += 1;
    }
  }

  // 当たり判定
  if (
    playerX < obstacleX + obstacleSize &&
    playerX + playerSize > obstacleX &&
    playerY < obstacleY + obstacleSize &&
    playerY + playerSize > obstacleY
  ) {
    gameOver = true;
  }
}

function draw() {
  ctx.clearRect(0, 0, WIDTH, HEIGHT);

  // プレイヤー
  ctx.fillStyle = 'black';
  ctx.fillRect(playerX, playerY, playerSize, playerSize);

  // 障害物
  ctx.fillStyle = 'red';
  ctx.fillRect(obstacleX, obstacleY, obstacleSize, obstacleSize);

  // スコア
  ctx.fillStyle = 'black';
  ctx.font = '24px Arial';
  ctx.fillText(`スコア: ${score}`, 10, 30);

  if (gameOver) {
    ctx.fillStyle = 'red';
    ctx.font = '48px Arial';
    ctx.fillText('ゲームオーバー！', WIDTH / 2 - 150, HEIGHT / 2);
  }
}

function gameLoop() {
  update();
  draw();
  if (!gameOver) {
    requestAnimationFrame(gameLoop);
  }
}

gameLoop();
</script>

</body>
</html>
