<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>CrazyGames Clone</title>
  <style>
    body {
      margin: 0;
      font-family: sans-serif;
      background: #f1f1f1;
    }
    header {
      background: #1d1d1d;
      color: white;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .logo {
      font-size: 1.5rem;
      font-weight: bold;
    }
    .search {
      padding: 0.5rem;
      width: 200px;
    }
    .games-container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1rem;
      padding: 2rem;
    }
    .game-card {
      background: white;
      border-radius: 8px;
      overflow: hidden;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      text-align: center;
      cursor: pointer;
      transition: transform 0.2s;
    }
    .game-card:hover {
      transform: translateY(-5px);
    }
    .game-card img {
      width: 100%;
      height: 140px;
      object-fit: cover;
    }
    .game-card h4 {
      margin: 0;
      padding: 0.5rem;
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">CrazyGames Clone</div>
    <input class="search" type="text" placeholder="Search games..." />
  </header>

  <main class="games-container">
    <div class="game-card" onclick="window.location.href='game.html'">
      <img src="https://via.placeholder.com/200x140" alt="Game 1" />
      <h4>Super Platformer</h4>
    </div>
    <div class="game-card" onclick="window.location.href='game.html'">
      <img src="https://via.placeholder.com/200x140" alt="Game 2" />
      <h4>Car Chase 3D</h4>
    </div>
    <div class="game-card" onclick="window.location.href='game.html'">
      <img src="https://via.placeholder.com/200x140" alt="Game 3" />
      <h4>Sniper Shooter</h4>
    </div>
  </main>
</body>
</html>
