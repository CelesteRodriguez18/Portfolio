# Celeste Rodríguez — Chatbot IA

## Estructura
```
celeste-chatbot/
├── server.js          ← backend Node.js
├── package.json
└── public/
    └── index.html     ← frontend completo
```

## Cómo correr localmente

1. Instalar dependencias:
```bash
npm install
```

2. Crear un archivo `.env` con tu API key de Anthropic:
```
ANTHROPIC_API_KEY=sk-ant-xxxxx
```

3. Correr el servidor:
```bash
npm start
```

4. Abrir http://localhost:3000

---

## Deploy en Railway (gratis, recomendado)

1. Crear cuenta en https://railway.app
2. Nuevo proyecto → "Deploy from GitHub repo"
3. Subir esta carpeta a un repo de GitHub
4. En Railway, ir a Variables y agregar:
   - `ANTHROPIC_API_KEY` = tu API key
5. Railway detecta el `package.json` y despliega automáticamente.
6. Te da una URL pública tipo `celeste-chatbot.up.railway.app`

## Obtener tu API key de Anthropic

1. Ir a https://console.anthropic.com
2. API Keys → Create Key
3. Copiar y pegar en Railway como variable de entorno

---

Tu API key NUNCA va en el código, siempre como variable de entorno.
