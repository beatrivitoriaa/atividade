# atividade
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Exercícios de Flexbox</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f0f0f0;
    }

    h1 {
      text-align: center;
      color: #4caf50;
      margin: 20px 0;
    }

    .container {
      display: flex;
      flex-wrap: wrap;
      padding: 20px;
      box-sizing: border-box;
      margin: 20px;
      background-color: #ffffff;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    .column {
      flex: 1; /* Largura igual */
      padding: 30px;
      box-sizing: border-box;
      background-color: #4caf50;
      color: white;
      margin: 10px; /* Espaçamento entre colunas */
      border-radius: 8px;
      text-align: center;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    .item {
      background-color: #4caf50;
      color: white;
      padding: 30px;
      margin: 10px; /* Espaçamento entre os itens */
      border-radius: 8px;
      display: flex;
      justify-content: center;
      align-items: center;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    .extra-item {
      background-color: #ff9800; /* Cor diferente para o item extra */
      flex: 2; /* Item extra ocupa o espaço restante */
    }

    .menu-item {
      margin: 10px 0;
      background-color: #4caf50;
      color: white;
      padding: 15px;
      border-radius: 8px;
      text-align: center;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    /* Estilos para os exercícios */
    .exercise {
      margin: 40px 0;
      padding: 20px;
      background-color: #ffffff;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }

    @media (max-width: 768px) {
      .column {
        flex-basis: 45%; /* Duas colunas em telas menores */
      }
    }

    @media (max-width: 480px) {
      .column {
        flex-basis: 100%; /* Uma coluna em telas muito pequenas */
      }
    }
  </style>
</head>
<body>

  <h1>Exercícios de Flexbox</h1>

  <!-- Exercício 1: Layout Básico -->
  <div class="exercise">
    <h2>Exercício 1: Layout Básico</h2>
    <div class="container">
      <div class="column">
        <h3>Coluna 1</h3>
        <p>Este é o conteúdo da coluna 1.</p>
      </div>
      <div class="column">
        <h3>Coluna 2</h3>
        <p>Este é o conteúdo da coluna 2.</p>
      </div>
      <div class="column">
        <h3>Coluna 3</h3>
        <p>Este é o conteúdo da coluna 3.</p>
      </div>
    </div>
  </div>

  <!-- Exercício 2: Alinhamento Vertical -->
  <div class="exercise">
    <h2>Exercício 2: Alinhamento Vertical</h2>
    <div class="container" style="height: 400px; align-items: center;">
      <div class="item" style="height: 100px;">Item 1</div>
      <div class="item" style="height: 150px;">Item 2</div>
      <div class="item" style="height: 200px;">Item 3</div>
    </div>
  </div>

  <!-- Exercício 3: Distribuição de Espaço -->
  <div class="exercise">
    <h2>Exercício 3: Distribuição de Espaço</h2>
    <div class="container" style="justify-content: space-between;">
      <div class="item">Item 1</div>
      <div class="item">Item 2</div>
      <div class="item">Item 3</div>
      <div class="item">Item 4</div>
      <div class="item extra-item">Item Extra</div>
    </div>
  </div>

  <!-- Exercício 4: Reordenação de Itens -->
  <div class="exercise">
    <h2>Exercício 4: Reordenação de Itens</h2>
    <div class="container">
      <div class="item" style="order: 2;">Item 1</div>
      <div class="item" style="order: 4;">Item 2</div>
      <div class="item" style="order: 1;">Item 3</div>
      <div class="item" style="order: 3;">Item 4</div>
      <div class="item" style="order: 5;">Item 5</div>
    </div>
  </div>

  <!-- Exercício 5: Layout Complexo com Flexbox -->
  <div class="exercise">
    <h2>Exercício 5: Layout Complexo</h2>
    <div style="display: flex; flex-direction: column; height: 100vh;">
      <header style="background-color: #4caf50; color: white; text-align: center; padding: 20px;">Header</header>
      <div style="display: flex; flex: 1;">
        <div class="container" style="width: 250px; background-color: #f0f0f0; padding: 20px; display: flex; flex-direction: column; justify-content: center;">
          <div class="menu-item">Menu 1</div>
          <div class="menu-item">Menu 2</div>
          <div class="menu-item">Menu 3</div>
        </div>
        <div style="flex: 1; padding: 20px; background-color: #ffffff;">
          <h3>Área de Conteúdo Principal</h3>
          <p>Este é o conteúdo principal da página.</p>
        </div>
      </div>
      <footer style="background-color: #4caf50; color: white; text-align: center; padding: 20px;">Footer</footer>
    </div>
  </div>

</body>
</html>
