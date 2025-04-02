# Olá! 🐱

```tsx
import React from "react";

interface DesenvolvedorProps {
  nome: string;
  habilidades: string[];
}

const Desenvolvedor: React.FC<DesenvolvedorProps> = ({ nome, habilidades }) => {
  return (
    <div style={{ padding: "20px", fontFamily: "Arial" }}>
      <h2>Nome: {nome}</h2>
      <p>Habilidades: {habilidades.join(", ")}</p>
    </div>
  );
};

const Aplicacao: React.FC = () => {
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

  return <Desenvolvedor nome={perfilDesenvolvedor.nome} habilidades={perfilDesenvolvedor.habilidades} />;
};

export default Aplicacao;
