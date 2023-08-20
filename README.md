```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
  body {
    background-color: black;
    color: white;
    font-family: Arial, sans-serif;
  }
  .container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
  h2 {
    font-size: 24px;
  }
  .buttons {
    display: flex;
    gap: 10px;
    margin-top: 10px;
  }
  .button {
    background-color: white;
    color: blue;
    border: 1px solid blue;
    border-radius: 5px;
    padding: 8px 15px;
    cursor: pointer;
  }
  .button:hover {
    background-color: blue;
    color: white;
  }
  #noButton {
    position: absolute;
  }
</style>
</head>
<body>
<div class="container">
  <h2>ff hoje?</h2>
  <div class="buttons">
    <a id="yesButton" href="https://youtu.be/ZAefvN72ctU" target="_blank" class="button">Sim</a>
    <button id="noButton" class="button">Não</button>
  </div>
</div>
<script>
  const noButton = document.getElementById('noButton');
  const yesButton = document.getElementById('yesButton');
  const container = document.querySelector('.container');

  yesButton.addEventListener('mouseenter', () => {
    yesButton.href = 'https://youtu.be/ZAefvN72ctU';
  });

  noButton.addEventListener('click', () => {
    const randomX = Math.random() * (container.offsetWidth - noButton.offsetWidth);
    const randomY = Math.random() * (container.offsetHeight - noButton.offsetHeight);
    noButton.style.left = randomX + 'px';
    noButton.style.top = randomY + 'px';
  });
</script>
</body>
</html>
```# laughing-pancake
Pedido para jogar irrecusável 
