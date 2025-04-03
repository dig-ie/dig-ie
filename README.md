```javascript
const express = require("express");
const app = express();
const port = 3000;

const perfilDesenvolvedor = {
  nome: "Diêgo de Barros",
  habilidades: [
    "Desenvolvedor Full Stack",
    "React",
    "React Native",
    "FlutterFlow",
    "TypeScript",
    "APIs REST",
    "GraphQL",
    "Node.js",
    "NestJS",
    ".NET",
    "Git",
    "GitHub",
    "Dart",
    "PostgreSQL",
    "MySQL",
    "NoSQL (MongoDB, MongoDB Atlas, Redis)",
    "AWS (Lambda, S3, DynamoDB)",
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
