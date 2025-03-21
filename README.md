<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Emprestar Dinheiro a Juros</title>
    <style>
        body {
            background-color: black;
            color: white;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #333;
            padding: 15px;
            text-align: center;
        }
        .form-container {
            margin: 20px;
            padding: 20px;
            background-color: #444;
            border-radius: 8px;
        }
        input, select, textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border-radius: 4px;
            border: 1px solid #ddd;
            background-color: #222;
            color: white;
        }
        button {
            padding: 10px 20px;
            margin: 10px 5px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        .button-blue {
            background-color: #007BFF;
            color: white;
        }
        .button-green {
            background-color: #28a745;
            color: white;
        }
        .chat-container {
            margin-top: 30px;
            background-color: #555;
            padding: 15px;
            border-radius: 8px;
        }
        .chat-box {
            width: 100%;
            height: 150px;
            background-color: #222;
            color: white;
            padding: 10px;
            border-radius: 5px;
            resize: none;
        }
        .chat-input {
            width: 100%;
            padding: 10px;
            margin-top: 10px;
            border-radius: 4px;
            border: 1px solid #ddd;
            background-color: #222;
            color: white;
        }
        .chat-button {
            margin-top: 10px;
            padding: 10px 20px;
            background-color: #28a745;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
    </style>
</head>
<body>

<header>
    <h1>Emprestar Dinheiro a Juros</h1>
</header>

<div class="form-container">
    <h2>Formulário de Empréstimo</h2>
    <form>
        <label for="nome">Nome Completo</label>
        <input type="text" id="nome" name="nome" required>

        <label for="valor">Valor do Empréstimo (R$)</label>
        <input type="number" id="valor" name="valor" required>

        <label for="taxa">Taxa de Juros (%)</label>
        <input type="number" id="taxa" name="taxa" required>

        <label for="prazo">Prazo (meses)</label>
        <input type="number" id="prazo" name="prazo" required>

        <button type="submit" class="button-blue">Solicitar Empréstimo</button>
        <button type="reset" class="button-green">Limpar Formulário</button>
    </form>
</div>

<div class="chat-container">
    <h2>Chat</h2>
    <textarea class="chat-box" readonly></textarea>
    <input type="text" class="chat-input" placeholder="Digite sua mensagem...">
    <button class="chat-button">Enviar</button>
</div>

</body>
</html>
