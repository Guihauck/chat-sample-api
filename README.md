# 💬 Flask Chat com Socket.IO

Este é um exemplo simples de aplicação web de chat em tempo real utilizando **Flask** e **Flask-SocketIO**. Os usuários conectados podem enviar mensagens que são transmitidas para todos os participantes instantaneamente.

## 🚀 Tecnologias Utilizadas

- [Python](https://www.python.org/)
- [Flask](https://flask.palletsprojects.com/)
- [Flask-SocketIO](https://flask-socketio.readthedocs.io/)
- [Socket.IO](https://socket.io/)
- HTML/CSS (com template `index.html`)

## 📦 Instalação

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/flask-chat-socketio.git
cd flask-chat-socketio
```

2. Crie um ambiente virtual (opcional, mas recomendado):

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
```

3. Instale as dependências:

```bash
pip install flask flask-socketio
```

## ▶️ Executando a aplicação

1. Certifique-se de ter o arquivo `index.html` dentro da pasta `templates/`.
2. Execute a aplicação com:

```bash
python app.py
```

3. Acesse no navegador:

```
http://localhost:5000
```

## 📁 Estrutura do Projeto

```
flask-chat-socketio/
├── app.py
├── templates/
│   └── index.html
└── README.md
```

## ✉️ Funcionalidade

- O servidor escuta por mensagens enviadas pelo cliente.
- Cada mensagem recebida é transmitida a **todos os clientes conectados** usando `broadcast=True`.
