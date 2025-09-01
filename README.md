# silverat-site
site futurista para venda de meta quest 128 gb via pix
# Silverat - Loja de VR
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Silverat - Meta Quest 2 128GB</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&display=swap');

  body {
    margin: 0;
    font-family: 'Orbitron', sans-serif;
    background: linear-gradient(120deg, #0f0c29, #302b63, #24243e);
    color: #fff;
    overflow-x: hidden;
  }

  header {
    text-align: center;
    padding: 2rem;
    background: rgba(0,0,0,0.7);
    box-shadow: 0 0 20px #00ffff;
  }

  header h1 {
    font-size: 3rem;
    color: #00ffff;
    text-shadow: 0 0 10px #00ffff, 0 0 20px #00ffff;
    animation: neonGlow 1.5s ease-in-out infinite alternate;
  }

  @keyframes neonGlow {
    from { text-shadow: 0 0 5px #00ffff, 0 0 10px #00ffff; }
    to { text-shadow: 0 0 20px #00ffff, 0 0 40px #00ffff; }
  }

  main {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 2rem;
  }

  .produto {
    display: flex;
    flex-direction: column;
    align-items: center;
    background: rgba(255,255,255,0.05);
    padding: 2rem;
    border-radius: 15px;
    max-width: 400px;
    text-align: center;
    box-shadow: 0 0 15px #00ffff;
    transition: transform 0.3s;
  }

  .produto:hover {
    transform: scale(1.05);
  }

  .produto img {
    width: 100%;
    border-radius: 10px;
    box-shadow: 0 0 15px #00ffff;
  }

  .produto h2 {
    color: #00ffff;
    margin: 1rem 0 0.5rem;
    text-shadow: 0 0 5px #00ffff;
  }

  .produto p {
    font-size: 1rem;
    margin: 0.5rem 0 1rem;
    color: #ccc;
  }

  .preco {
    font-size: 1.5rem;
    margin-bottom: 1rem;
    color: #ffcc00;
    text-shadow: 0 0 5px #ffcc00;
  }

  .botao-pix {
    background: linear-gradient(45deg, #00ffff, #00e5e5);
    color: #000;
    padding: 1rem 2rem;
    font-size: 1.3rem;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    transition: 0.3s;
    box-shadow: 0 0 10px #00ffff;
  }

  .botao-pix:hover {
    transform: scale(1.1);
    box-shadow: 0 0 25px #00ffff;
  }

  footer {
    text-align: center;
    padding: 1rem;
    background: rgba(0,0,0,0.7);
    margin-top: 2rem;
    box-shadow: 0 0 15px #00ffff;
  }
</style>
</head>
<body>
<header>
  <h1>Silverat</h1>
  <p>Compre o Meta Quest 2 128GB agora!</p>
</header>
<main>
  <div class="produto">
    <img src="meta_quest.jpg" alt="Meta Quest 2 128GB">
    <h2>Meta Quest 2 - 128GB</h2>
    <p>O headset de realidade virtual mais avançado, agora disponível na Silverat.</p>
    <div class="preco">R$ 3.499,00</div>
    <button class="botao-pix" onclick="comprarPix()">Comprar com Pix</button>
  </div>
</main>
<footer>
  &copy; 2025 Silverat. Todos os direitos reservados.
</footer>

<script>
function comprarPix() {
  const pix = "21967827712";
  const valor = "3499.00";
  const mensagem = encodeURIComponent("Compra do Meta Quest 2 128GB - Silverat");
  const link = `https://api.whatsapp.com/send?phone=55${pix}&text=${mensagem}%20R$${valor}`;
  window.open(link, "_blank");
}
</script>
</body>
</html>
