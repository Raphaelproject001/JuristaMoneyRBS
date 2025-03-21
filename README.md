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
    text-decoration
