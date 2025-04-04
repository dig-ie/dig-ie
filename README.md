```javascript
const express = require("express");
const app = express();
const port = 3000;

const perfilDesenvolvedor = {
  nome: "Diêgo de Barros",
  habilidades: [
    "Desenvolvedor Full Stack",
    "React",
    "FlutterFlow",
    "React Native",
    "Dart",
    "TypeScript",
    "APIs REST/RESTful",
    "Node.js",
    "NestJS",
    ".NET",
    "Git",
    "GitHub",
    "PostgreSQL",
    "MySQL",
    "NoSQL (MongoDB, MongoDB Atlas, Redis)",
    "GCP",
    "Supabase",
    "Docker",
    "CI/CD (GitHub Actions, Vercel)"
  ],
};

app.get("/desenvolvedor", (req, res) => {
  res.json(perfilDesenvolvedor);
});

app.listen(port, () => {
  console.log(`Servidor rodando em http://localhost:${port}`);
});
