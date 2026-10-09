<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bot AI - Dashboard & Auth</title>
    <style>
        /* CSS3 - Estilos Globais e Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #0f172a;
            color: #f8fafc;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }

        .container {
            width: 100%;
            max-width: 450px;
            background: #1e293b;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.5);
        }

        .dashboard-container {
            max-width: 800px;
            width: 90%;
            height: 85vh;
            display: flex;
            flex-direction: column;
        }

        h2 {
            margin-bottom: 20px;
            text-align: center;
            color: #38bdf8;
        }

        .input-group {
            margin-bottom: 15px;
        }

        .input-group label {
            display: block;
            margin-bottom: 5px;
            font-size: 14px;
            color: #94a3b8;
        }

        .input-group input {
            width: 100%;
            padding: 10px;
            border: 1px solid #334155;
            border-radius: 6px;
            background: #0f172a;
            color: #fff;
            font-size: 16px;
        }

        .input-group input:focus {
            outline: none;
            border-color: #38bdf8;
        }

        button {
            width: 100%;
            padding: 12px;
            background: #38bdf8;
            border: none;
            border-radius: 6px;
            color: #0f172a;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            transition: background 0.3s;
        }

        button:hover {
            background: #0ea5e9;
        }

        .switch-form {
            margin-top: 15px;
            text-align: center;
            font-size: 14px;
            color: #94a3b8;
        }

        .switch-form a {
            color: #38bdf8;
            text-decoration: none;
        }

        /* Dashboard de Chat */
        .chat-box {
            flex: 1;
            background: #1e293b;
            border-radius: 12px 12px 0 0;
            padding: 20px;
            overflow-y: auto;
            border: 1px solid #334155;
        }

        .input-area {
            display: flex;
            background: #1e293b;
            padding: 15px;
            border-radius: 0 0 12px 12px;
            border: 1px solid #334155;
            border-top: none;
            gap: 10px;
        }

        .input-area input {
            flex: 1;
            padding: 12px;
            background: #0f172a;
            border: 1px solid #334155;
            border-radius: 6px;
            color: #fff;
        }

        .input-area button {
            width: auto;
            padding: 0 25px;
        }

        .message {
            margin-bottom: 15px;
            padding: 12px;
            border-radius: 8px;
            max-width: 80%;
        }

        .message.user {
            background: #334155;
            margin-left: auto;
            color: #fff;
        }

        .message.bot {
            background: #0f172a;
            margin-right: auto;
            border-left: 4px solid #38bdf8;
        }

        .badge {
            display: inline-block;
            padding: 2px 6px;
            font-size: 11px;
            font-weight: bold;
            border-radius: 4px;
            margin-bottom: 5px;
            text-transform: uppercase;
        }

        .badge.foto { background: #ec4899; color: #fff; }
        .badge.video { background: #eab308; color: #0f172a; }
        .badge.programacao { background: #22c55e; color: #fff; }

        pre {
            background: #1e293b;
            padding: 10px;
            border-radius: 6px;
            overflow-x: auto;
            font-family: 'Courier New', Courier, monospace;
            color: #a7f3d0;
        }

        .hidden {
            display: none !important;
        }
    </style>
</head>
<body>

    <!-- TELA DE AUTENTICAÇÃO (CADASTRO / LOGIN) -->
    <div id="auth-section" class="container">
        <!-- Formulário de Cadastro -->
        <div id="register-form">
            <h2>Criar Conta - Bot AI</h2>
            <div class="input-group">
                <label>Nome Completo</label>
                <input type="text" id="reg-name" placeholder="Seu nome">
            </div>
            <div class="input-group">
                <label>E-mail (Apenas gmail, hotmail ou email.com)</label>
                <input type="email" id="reg-email" placeholder="seu@email.com">
            </div>
            <div class="input-group">
                <label>Senha</label>
                <input type="password" id="reg-password" placeholder="Sua senha">
            </div>
            <button onclick="handleRegister()">Cadastrar</button>
            <div class="switch-form">
                Já tem uma conta? <a href="#" onclick="toggleForm(false)">Faça Login</a>
            </div>
        </div>

        <!-- Formulário de Login -->
        <div id="login-form" class="hidden">
            <h2>Login - Bot AI</h2>
            <div class="input-group">
                <label>E-mail</label>
                <input type="email" id="login-email" placeholder="seu@email.com">
            </div>
            <div class="input-group">
                <label>Senha</label>
                <input type="password" id="login-password" placeholder="Sua senha">
            </div>
            <button onclick="handleLogin()">Entrar</button>
            <div class="switch-form">
                Não tem uma conta? <a href="#" onclick="toggleForm(true)">Cadastre-se</a>
            </div>
        </div>
    </div>

    <!-- TELA DO CHAT (BOT AI DASHBOARD) -->
    <div id="dashboard-section" class="dashboard-container hidden">
        <h2>🤖 Painel Bot AI</h2>
        <div class="chat-box" id="chat-box">
            <div class="message bot">
                Olá! Eu sou o Bot AI. Digite o que você precisa (ex: uma foto de um gato, um vídeo da praia ou um código de calculadora).
            </div>
        </div>
        <div class="input-area">
            <input type="text" id="user-prompt" placeholder="Digite seu comando aqui..." onkeypress="checkEnter(event)">
            <button onclick="processPrompt()">Enviar</button>
        </div>
    </div>

    <script>
        /* JAVASCRIPT - Lógica de Autenticação e Banco de Dados (LocalStorage) */
        function toggleForm(showRegister) {
            document.getElementById('register-form').classList.toggle('hidden', !showRegister);
            document.getElementById('login-form').classList.toggle('hidden', showRegister);
        }

        function validateEmailProvider(email) {
            const allowedProviders = ['@gmail.com', '@hotmail.com', '@email.com'];
            return allowedProviders.some(provider => email.toLowerCase().endsWith(provider));
        }

        function handleRegister() {
            const name = document.getElementById('reg-name').value.trim();
            const email = document.getElementById('reg-email').value.trim();
            const password = document.getElementById('reg-password').value.trim();

            if (!name || !email || !password) {
                alert('Por favor, preencha todos os campos!');
                return;
            }

            if (!validateEmailProvider(email)) {
                alert('Erro: Cadastros válidos apenas para provedores @gmail.com, @hotmail.com ou @email.com!');
                return;
            }

            // Simulação de verificação no banco de dados local
            let users = JSON.parse(localStorage.getItem('bot_ai_users')) || [];
            if (users.some(u => u.email === email)) {
                alert('Este e-mail já está cadastrado!');
                return;
            }

            users.push({ name, email, password });
            localStorage.setItem('bot_ai_users', JSON.stringify(users));
            alert('Cadastro realizado com sucesso! Faça seu login.');
            toggleForm(false);
        }

        function handleLogin() {
            const email = document.getElementById('login-email').value.trim();
            const password = document.getElementById('login-password').value.trim();

            let users = JSON.parse(localStorage.getItem('bot_ai_users')) || [];
            const user = users.find(u => u.email === email && u.password === password);

            if (user) {
                document.getElementById('auth-section').classList.add('hidden');
                document.getElementById('dashboard-section').classList.remove('hidden');
            } else {
                alert('E-mail ou senha incorretos!');
            }
        }

        function checkEnter(event) {
            if (event.key === 'Enter') processPrompt();
        }

        /* JAVASCRIPT - Scanner de Prompt e Direcionamento de API */
        function scanPrompt(prompt) {
            const text = prompt.toLowerCase();
            
            // Palavras-chave do scanner
            const keywordsProgramming = ['codigo', 'código', 'programacao', 'programação', 'funcao', 'função', 'javascript', 'html', 'css', 'python', 'script', 'algoritmo', 'desenvolva'];
            const keywordsVideo = ['video', 'vídeo', 'animacao', 'animação', 'filme', 'take', 'clipe', 'gravacao', 'gravação'];
            const keywordsPhoto = ['foto', 'imagem', 'desenho', 'ilustracao', 'ilustração', 'retrato', 'pintura', 'fotografia', 'banner'];

