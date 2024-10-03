<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Snake Game with Score</title>
  <style>
    html, body {
      height: 100%;
      margin: 0;
      background-color: black;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    canvas {
      border: 1px solid white;
    }

    .scoreboard {
      color: white;
      text-align: center;
      margin-bottom: 10px;
    }
  </style>
</head>
<body>

  <div class="scoreboard">
    <div>Current Score: <span id="current-score">0</span></div>
    <div>High Score: <span id="high-score">0</span></div>
  </div>
  <canvas id="game" width="400" height="400"></canvas>

  <script>
    var currentScoreElement = document.getElementById('current-score');
    var highScoreElement = document.getElementById('high-score');

    var currentScore = 0;
    var highScore = localStorage.getItem('highScore') || 0;
    highScoreElement.textContent = highScore;

    var canvas = document.getElementById('game');
    var context = canvas.getContext('2d');

    var grid = 16;
    var count = 0;

    var snake = {
      x: 160,
      y: 160,
      dx: grid,
      dy: 0,
      cells: [],
      maxCells: 4
    };

    var apple = {
      x: 320,
      y: 320
    };

    function getRandomInt(min, max) {
      return Math.floor(Math.random() * (max - min)) + min;
    }

    function loop() {
      requestAnimationFrame(loop);

      if (++count < 4) {
        return;
      }

      count = 0;
      context.clearRect(0, 0, canvas.width, canvas.height);

      snake.x += snake.dx;
      snake.y += snake.dy;

      if (snake.x < 0) {
        snake.x = canvas.width - grid;
      } else if (snake.x >= canvas.width) {
        snake.x = 0;
      }

      if (snake.y < 0) {
        snake.y = canvas.height - grid;
      } else if (snake.y >= canvas.height) {
        snake.y = 0;
      }

      snake.cells.unshift({ x: snake.x, y: snake.y });

      if (snake.cells.length > snake.maxCells) {
        snake.cells.pop();
      }

      context.fillStyle = 'red';
      context.fillRect(apple.x, apple.y, grid - 1, grid - 1);

      context.fillStyle = 'green';
      snake.cells.forEach(function (cell, index) {
        context.fillRect(cell.x, cell.y, grid - 1, grid - 1);

        if (cell.x === apple.x && cell.y === apple.y) {
          snake.maxCells++;
          currentScore++;
          currentScoreElement.textContent = currentScore;

          if (currentScore > highScore) {
            highScore = currentScore;
            highScoreElement.textContent = highScore;
            localStorage.setItem('highScore', highScore);
          }

          apple.x = getRandomInt(0, 25) * grid;
          apple.y = getRandomInt(0, 25) * grid;
        }

        for (var i = index + 1; i < snake.cells.length; i++) {
          if (cell.x === snake.cells[i].x && cell.y === snake.cells[i].y) {
            snake.x = 160;
            snake.y = 160;
            snake.cells = [];
            snake.maxCells = 4;
            snake.dx = grid;
            snake.dy = 0;

            currentScore = 0;
            currentScoreElement.textContent = currentScore;

            apple.x = getRandomInt(0, 25) * grid;
            apple.y = getRandomInt(0, 25) * grid;
          }
        }
      });
    }

    document.addEventListener('keydown', function (e) {
      if (e.which === 37 && snake.dx === 0) {
        snake.dx = -grid;
        snake.dy = 0;
      } else if (e.which === 38 && snake.dy === 0) {
        snake.dy = -grid;
        snake.dx = 0;
      } else if (e.which === 39 && snake.dx === 0) {
        snake.dx = grid;
        snake.dy = 0;
      } else if (e.which === 40 && snake.dy === 0) {
        snake.dy = grid;
        snake.dx = 0;
      }
    });

    requestAnimationFrame(loop);
  </script>
</body>
</html>
