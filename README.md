<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <title>Comandos com Botão de Copiar</title>
  <style>
    body {
      background-color: #111;
      color: #0f0;
      font-family: monospace;
      padding: 20px;
    }
    .comando-container {
      position: relative;
      background: #000;
      border: 1px solid #0f0;
      padding: 10px 50px 10px 10px;
      margin-bottom: 15px;
      border-radius: 8px;
      overflow-x: auto;
    }
    .copiar-btn {
      position: absolute;
      top: 8px;
      right: 8px;
      background-color: #0f0;
      color: #000;
      border: none;
      padding: 5px 10px;
      border-radius: 5px;
      cursor: pointer;
      font-weight: bold;
    }
    .copiar-btn:hover {
      background-color: #00ff88;
    }
    code {
      display: block;
      white-space: pre;
    }
    img {
      max-width: 100%;
      border: 1px solid #0f0;
      border-radius: 6px;
      margin: 15px 0;
    }
  </style>
</head>
<body>

<h2>Comandos para executar o ALFAZ_DDOS</h2>

<div class="comando-container">
  <code id="cmd1">pkg install python3</code>
  <button class="copiar-btn" onclick="copiarTexto('cmd1')">Copiar</button>
</div>

<div class="comando-container">
  <code id="cmd2">pkg install git</code>
  <button class="copiar-btn" onclick="copiarTexto('cmd2')">Copiar</button>
</div>

<div class="comando-container">
  <code id="cmd3">rm -rf alfaz_ddos</code>
  <button class="copiar-btn" onclick="copiarTexto('cmd3')">Copiar</button>
</div>

<div class="comando-container">
  <code id="cmd4">chmod +x *</code>
  <button class="copiar-btn" onclick="copiarTexto('cmd4')">Copiar</button>
</div>

<div class="comando-container">
  <code id="cmd5">git clone https://github.com/mdalfaz/alfaz_ddos.git</code>
  <button class="copiar-btn" onclick="copiarTexto('cmd5')">Copiar</button>
</div>

<div class="comando-container">
  <code id="cmd6">cd alfaz_ddos</code>
  <button class="copiar-btn" onclick="copiarTexto('cmd6')">Copiar</button>
</div>

<div class="comando-container">
  <code id="cmd7">ls</code>
  <button class="copiar-btn" onclick="copiarTexto('cmd7')">Copiar</button>
</div>

<div class="comando-container">
  <code id="cmd8">python3 setup.py</code>
  <button class="copiar-btn" onclick="copiarTexto('cmd8')">Copiar</button>
</div>

<img src="https://github.com/mdalfaz/alfaz_ddos/assets/125147223/50b58114-17ca-462e-a6bf-39f3218feca4" alt="Screenshot Setup">

<div class="comando-container">
  <code id="cmd9">python3 ddos.py</code>
  <button class="copiar-btn" onclick="copiarTexto('cmd9')">Copiar</button>
</div>

<img src="https://github.com/mdalfaz/alfaz_ddos/assets/125147223/93c6cfdc-5ab9-4dd8-a525-dd117681a012" alt="Screenshot Ataque">

<div class="comando-container">
  <code id="cmd10">python3 ddos2.py</code>
  <button class="copiar-btn" onclick="copiarTexto('cmd10')">Copiar</button>
</div>

<img src="https://github.com/mdalfaz/ALFAZ_DDOS/assets/125147223/bfdac383-af99-415a-baed-1ce6fcb421e3" alt="ddos2 Screenshot 1">
<img src="https://github.com/mdalfaz/ALFAZ_DDOS/assets/125147223/910b2761-10b9-42e9-a6de-2628c35efd12" alt="ddos2 Screenshot 2">
<img src="https://github.com/mdalfaz/ALFAZ_DDOS/assets/125147223/2aad625e-a580-4202-83ab-69c517ce5444" alt="ddos2 Screenshot 3">

<script>
  function copiarTexto(id) {
    const texto = document.getElementById(id).innerText;
    navigator.clipboard.writeText(texto).then(() => {
      alert("Comando copiado!");
    });
  }
</script>

</body>
</html>
