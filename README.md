<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Empréstimos Online</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Cabeçalho -->
    <header>
        <nav>
            <ul>
                <li><a href="#home">Início</a></li>
                <li><a href="#servicos">Empréstimos</a></li>
                <li><a href="#agendamento">Agendar</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
    </header>

    <!-- Seção de Empréstimos -->
    <section id="servicos">
        <h1>Empréstimos Rápidos</h1>
        <p>Solicite seu empréstimo online de forma simples e segura.</p>
        <button class="btn" id="btnSolicitar">Solicitar Empréstimo</button>
    </section>

    <!-- Formulário de Agendamento -->
    <section id="agendamento">
        <h2>Agende uma Consultoria</h2>
        <form id="formAgendamento">
            <label for="nome">Nome:</label>
            <input type="text" id="nome" name="nome" required>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>

            <label for="data">Data do Agendamento:</label>
            <input type="date" id="data" name="data" required>

            <button type="submit">Agendar</button>
        </form>
    </section>

    <!-- Chat -->
    <section id="chat">
        <div id="chat-box">
            <h3>Atendimento Online</h3>
            <div id="chat-messages"></div>
            <input type="text" id="chat-input" placeholder="Digite sua mensagem...">
            <button onclick="enviarMensagem()">Enviar</button>
        </div>
    </section>

    <!-- Rodapé -->
    <footer>
        <p>&copy; 2025 Empréstimos Online | Todos os direitos reservados.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
