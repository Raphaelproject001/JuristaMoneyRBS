<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Empréstimos Jurídicos</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Header -->
    <header>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Sobre</a></li>
                <li><a href="#">Simular Empréstimo</a></li>
                <li><a href="#">Login</a></li>
            </ul>
        </nav>
    </header>

    <!-- Seção Principal -->
    <section class="main-section">
        <h1>Empréstimos Jurídicos Facilitados</h1>
        <p>Obtenha o financiamento que você precisa para dar continuidade aos seus processos jurídicos.</p>
        <button onclick="window.location.href='simulacao.html'">Simule seu Empréstimo</button>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 Empréstimos Jurídicos. Todos os direitos reservados.</p>
    </footer>
</body>
</html>

/* Resetando margens e padding */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Corpo do documento */
body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f9;
    color: #333;
}

/* Header */
header {
    background-color: #003366;
    padding: 20px;
}

header nav ul {
    list-style-type: none;
    display: flex;
    justify-content: flex-start;
}

header nav ul li {
    margin-right: 20px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

/* Seção Principal */
.main-section {
    text-align: center;
    margin: 50px 0;
}

.main-section h1 {
    font-size: 2.5em;
    color: #003366;
}

.main-section p {
    font-size: 1.2em;
    margin: 20px 0;
}

.main-section button {
    padding: 15px 30px;
    font-size: 1.2em;
    background-color: #003366;
    color: white;
    border: none;
    cursor: pointer;
}

.main-section button:hover {
    background-color: #0055cc;
}

/* Footer */
footer {
    text-align: center;
    background-color: #003366;
    color: white;
    padding: 20px 0;
}
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simulação de Empréstimo</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Header -->
    <header>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Sobre</a></li>
                <li><a href="#">Simular Empréstimo</a></li>
                <li><a href="#">Login</a></li>
            </ul>
        </nav>
    </header>

    <!-- Formulário de Simulação -->
    <section class="simulacao-section">
        <h1>Simule Seu Empréstimo</h1>
        <form id="form-simulacao">
            <label for="valor">Valor do Empréstimo:</label>
            <input type="number" id="valor" name="valor" required>

            <label for="prazo">Prazo (meses):</label>
            <input type="number" id="prazo" name="prazo" required>

            <button type="submit">Calcular Parcelas</button>
        </form>

        <div id="resultado" style="display:none;">
            <h2>Resultado da Simulação</h2>
            <p id="parcelas"></p>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 Empréstimos Jurídicos. Todos os direitos reservados.</p>
    </footer>

    <script>
        // Função de simulação de empréstimo
        document.getElementById("form-simulacao").addEventListener("submit", function(event) {
            event.preventDefault();

            // Obtendo valores dos inputs
            const valor = parseFloat(document.getElementById("valor").value);
            const prazo = parseInt(document.getElementById("prazo").value);

            // Simulação de juros (ex: 2% ao mês)
            const taxaJuros = 0.02;
            const valorTotal = valor * Math.pow(1 + taxaJuros, prazo);
            const parcelas = valorTotal / prazo;

            // Exibindo o resultado
            document.getElementById("parcelas").textContent = `Valor das parcelas: R$ ${parcelas.toFixed(2)} por ${prazo} meses.`;
            document.getElementById("resultado").style.display = "block";
        });
    </script>
</body>
</html>
